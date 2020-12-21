+++
title = "prep.gg - gaming, stats, and cloud pub/sub "
description = ""
tags = [
    "esports",
    "projects",
    "hackathon"
]
date = "2020-11-08"
categories = [
    "education",
    "career",
]
+++

As my friends know, I love to watch league of legends esports in my spare time, somewhat ashamedly. The excitement of watching pros play a video game I enjoy at the highest level is hard to describe. I distinctly remember sophomore year stumbling upon some classmates watching an esports finals in a dorm lounge. Now, 3 years later, I find myself consuming any piece of esports content I can get my hands on.

It was just a quirky passion in my mind though, like knitting or skiing. I majored in cs in college, so I always wondered what lies at the intersection of cs and esports. This past September, I saw that Team Liquid, one of the premier esport organizations, was hosting a hackathon. I immediately asked my friend, Dan, an MIT classmate who shares my passion of esports and analytics, to apply and see what we can build in 2 days. 

The result: [**prep.gg**](http://www.prep.gg/), a dashboard for pro teams to analyze their opponents.

## prep.gg

Concept: we wanted to build a one-stop analytics website that displays all relevant stats about a professionl League team. This include win rates, champion pick & ban rates, gold shares, etc. Normally, coaches have to manually collect such intel through VODs, and compile trends in jank excel sheets. Turns out, most of this data is publicly available, saving us the trouble of some fancy computer-vision data-extraction venture. That means technically, it's possible scrap all the data... 

Right?

Turns out, this project is pretty straightforward. Below is a view of TSM's 2020 League of Legends team stats on prep.gg:

![me](/img/prepgg/team_view.jpg)

![me](/img/prepgg/team_view2.jpg)

Users can easily navigate to any team from the home page:

![me](/img/prepgg/home_view.jpg)

(And yes, we did decide to use Teemo as our mascot)

## The Boring Stuff: How We Built Everything

Technical details aren't the most interesting, so I'll keep this concise (:

### Automating Data Aggregation with Cloud Pub/Sub

We find that a ton of the stats people are interested in are available on websites such as [Leaguepedia](https://lol.gamepedia.com/League_of_Legends_Esports_Wiki) and [Game Of Legends Esports](https://gol.gg/esports/home/), albeit in hard-to-read formats. These stats are updated regularly as the season progresses. To collect data from these sites, we use a combination of selenium browser automation and Python BeautifulSoup to scrap the data and aggregate it in a JSON format. We store these JSON files in an AWS S3 bucket. Since we want these to be as up to date as possible, we regularly automate our scraping with a Cloud Pub/Sub architecture on AWS. More specifically, we schedule a publish event once a day, and the cron job subscribed to this topic that does our scraping is triggered. This is achieved through AWS Cloudwatch and Lambda. This takes the pain out of manually collecting the data every time we need more up-to-date data.

Now that all the data we need is stored in a bucket, we can readily access the JSON via HTTP, and let the server/front-end handle the rest. Data engineering is doneeeee.

### The Front End

This is historically my weakness, so, like I usually do for other projects that I want to look nice without too much work, I looked around the internet for a nice Bootstrap/HTML5 template as a starting point. Once I found opne that suits my use case, I host it on a Flask server, which acquires all the data, and passes these to the frontend for Javascript client-side rendering. Something something, Charts.js is pretty. All this is hosted on AWS Elastic Beanstalk.

### Security

AWS IAM roles. 'Nuff said.



## Cool Story Bro... What's Next?

Gooood question. 

First, I'd like to have a certificate for the site, because "Not Secure" websites look mad sketch and unprofessional. In addition, since the data we collect is dependent on teams having played games, it's hard for the site to function in the offseason, aka now. Welp. Still thinking about solutions atm.

It's also pretty useful to filter team statistics based on dates, patches, tournament, etc. Currently, we haven't found a website that provides these stats broken down by these categories, so we'll have to find new data vendors. Morale of the story, if the data is somewhere on the internet, we can probably scrape it.

Once that is all done... maybe we'll send it to pro teams to use? Fingers crossed. For now, this project's in an awkward phase of being more than a hackathon project, and less than a product.

## Takeaways

Biggest takeaway for me is how powerful the combination of selenium browser automation with a Cloud Pub/Sub architecture is. Theoretically, if properly engineered, this combination can provide a global API for any data on the internet. Developers clarify the data that they're looking for, and the system can simply subscribe the developer's endpoint to a particular topic, where publishes correspond to scraping events. 

I feel like I'm onto something here. More projects & writeups on this soon.


*Thanks to [Dan Rigobon](https://drigobon.com/) for being an amazing project partner.*