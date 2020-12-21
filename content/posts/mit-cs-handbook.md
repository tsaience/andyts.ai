+++
title = "a (subjective?) handbook on majoring in cs @ mit"
description = ""
tags = [
    "mit",
    "education",
    "instructive"
]
date = "2020-05-28"
categories = [
    "education",
    "career",
]
+++

Having spent the last five years at MIT pursuing undergrad & masters degrees in cs, I want to write a handbook that I wish I had as a freshman.

**Disclaimer**: This is mostly about pure cs at MIT (course 6-3); MIT has a eecs major (course 6-2), but since that wasn't my major, only parts that overlap with 6-3 are addressed. While I try to be objective, these are, at its core, opinions. This handbook assumes students have no prior knowledge of cs. For non-MIT readers, many mentioned classes are availble on MIT OCW, and some of the advice may be useful for anyone learning cs.



## MIT Coursework

MIT has many classes, but not all classes are equal in difficulty. The class credit count is a rough indicator of how time-consuming a class is, but there are 12 unit classes that are harder than 18 credit classes, so take the unit count with a grain of salt. When in doubt, word-of-mouth is probably the most accurate gauge of class difficulty. 

### Intro Classes

For those with absolutely no background in cs, **6.0001/2 Introduction to Computer Science & Programming in Python** is a gentle introduction to coding in Python. Students usually enjoy the class while not finding it super difficult. This class is friendly to non-cs-major students and helps fulfill credits for a cs minor.

Students who are more certain of their cs interest should take **6.08 Introduction to EECS via Interconnected Embedded Systems**, one of the more well-taught classes at MIT. The class has weekly labs that allow students to get live hands-on experience building, coding, and debugging, fundamental skills that will be used over and over again. The class has an army of TAs and LAs that are extremely helpful, and most students thoroughly enjoy the class.

As a side note, **6.02 Introduction to EECS via Communication Networks** is also a well-taught lab, where students learn about basics of communicating data. Similar to **6.08**, this is a in-class lab class. Material in this class comes up in systems classes later on, such as **6.033**, **6.857/8**, etc.

### Foundation Classes

Right off the bat, CS freshmen should take **6.006 Introduction to Algorithms** asap, because it is immediately applicable to to technical interviews. Those who take 6.006 early often get freshman / sophomore year internships, a major advantage going forward.

Another important class  is **6.009 Fundamentals of Programming**. Taught in Python, this class challenges students to solve problems with concepts ubiquitously used in CS, such as recursion, basic OOP & graph search. This class is also extremely helpful in preparing for technical interviews, since most interviews happen in Python; exam questions in the class are basically lengthened interview questions. 

**6.004 Computation Structures**, while not immediately applicable to most coding interviews, is one of my favorite classes. This class essentially teaches students what a computer is and how it is built; I found the material most useful in computer systems work later down the line. 

Together, these 3 classes form the foundation of cs students' knowledge at mit. The sooner students take any of these classes, the earlier they can explore specific interests within cs.

### Header Classes

Foundation classes all have a followup course. **6.046 Design and Analysis of Algorithms** follows after **6.006**. This is one of the hardest required classes as a cs major. But if you loved algorithms in 6.006, this should be a challenging and fun class. I had a great time in the class, but it was definitely challenging. Take this asap if you enjoyed 6.006 a lot.

**6.031 Elements of Software Construction** follows **6.009**. The class is 6.009 in Java, but instead of focusing on how to implement algorithmic concepts, it focuses more on writing careful test cases and a deeper dive into OOP. Labs are time-consuming but not difficult. Make sure to budget enough time for labs, since writing the test cases can take some time. They take students' test cases and run it on faulty implementations to see if the test cases would catch particular bugs. Be careful, the in-class nanoquizes are out to get you. This was my least favorite class during my time at MIT.

**6.033 Computer Systems Engineering** is the followup on **6.004**. This class is a discussions-based paper-reading class, and this will be the first of many computer systems classes that are papers-based. This class basically sets up students to take advanced computer systems classes.

Students usually take one of **6.034 Artificial Intelligence** or **6.036 Machine Learning**. From experience and word-of-mouth during my time, **6.034** was considerably easier than **6.036**. **6.034** is front-loaded, but has an extremely lenient exam policy during the time that Patrick Winston taught the class (rip). **6.036** has often been said to be poorly taught, but explores essential concepts in machine learning, an extremely popular field, making it one of the most popular classes at MIT.

### Advanced Classes

After header classes, students have a lot of flexibility in pursuing what classes they want to take. Advanced classes can mostly be divided into systems classes and math-based classes, though other specialized advanced classes exist. Systems classes build upon concepts explored in **6.004** and **6.033** while math-based classes build upon **6.046** or **6.034/6.036**. Students usually pursue advanced classes mostly concentrated in one of these concentrations, though many students take classes in both at some point. I was lucky enough to have taken a number of classes in both concentrations.

#### Advanced Systems Classes

Advanced systems classes are my favorite classes during my time at MIT. Most MIT systems classes involve reading lots of papers, implementing time-consuming and informative labs, are well-organized, taught by the same instructors, and stay relatively consistent throughout the years. The most popular ones include, but are not limited to the following classes:

* **6,172 Performance Engineering**
* **6.035 Compilers**
* **6.828 Operating Systems**
* **6.824 Distributed Systems**
* **6.858 Computer Systems Security**
* **6.857 Computer Network Security**
* **6.829 Computer Networks**

I heavily recommend **6.172 Performance Engineering**, which teaches students how to write code that runs fast. As someone who interned in and am returning to fintech, this course was essential to my day-to-day. In addition, **6.824 Distributed Systems** is my all-time-favorite class at MIT, taught by the famous Robert Morris. Students learn about distributed systems by building MapReduce, Raft, and sharded key-value servers. If I have to recommend only 2 classes at MIT, I would recommend **6.172** and **6.824**.

Generally, how much a student gets out of advanced systems classes scales well with the amount of time invested. I recommend not having a busy schedule when taking these classes.

#### Advanced Algorithm / Math-Based Classes

Advanced algorithm / math-based classes are heavily theoretical and involve little to no coding. Some of the most popular ones include, but are not limited to the following classes:

* **6.867 Machine Learning**
* **6.437 Inference and Information**
* **6.438 Algorithms in Inference**
* **6.854 Advanced Algorithms**
* **6.853 Topcs in Algorithmic Game Theory**
* **6.840 Theory of Computation**
* **6.860 Statistical Learning Theory and Applications**

As a whole, without a solid math background, these classes are rather challenging. Problem sets often take 10-20 hours, and exams are known to be notoriously difficult for most people. I *heavily* recommend getting a good linear algebra background before taking any of these classes. Make sure to attend recitation, since new concepts are introduced weekly, and recitation exercises often resemble exam questions. Many IMO and IOI medalists take these classes. Unfortunately, due to this advanced level of the classes, some classes may test material that is tangentially related to the course material but not explicitly taught, and exam questions may require mathematical synthesis or derivation. Try taking **6.867**, a good class on general machine learning, and if you enjoy it, you will likely enjoy most other topics on this list.

### Other Recommended Coursework

These are some classes I have heard great things about and would have taken if given the chance, but do not easily fit into the aforementioned categories.

* **6.837 Computer Graphics**. Self explanatory class name. General reviews have been positive.
* **6.864 Advanced NLP**. Heard to be difficult and rewarding, a mix of theoretical and implementation knowledge.
* **6.875 Cryptography and Cryptanalysis**. Became fascinated with the class after learning about encryption in security. Math-heavy, but included in this list due to applications in cybersecurity.
* **6.865 Digital and Computational Photography**. A unique class about applications of cs in photography. Highly recommended from all those I know who have taken the class.

### Classes Tier List

I compiled a tier list of classes below as a summary. I consulted a few friends to compile this tier list. These rankings are subjective, but the tier list should be accurate to ± 1 tier based on talking to my MIT friends.

* **S-tier**: 6.172, 6.824, 6.828
* **A-tier**: 6.08, 6.006, 6.004, 6.858, 6.009, 6.046
* **B-tier**: 6.034, 6.0001/2, 6.437, 6.867
* **C-tier**: 6.035, 6.033, 6.438, 6.853, 6.036



## Research

MIT provides its students with unique opportunities to work with its world-class professors through **UROP (undergraduate research opportunities program)**. Students in cs usually urop in MIT CSAIL (Computer Science and AI Labs) or MIT Media Lab. MIT CSAIL has many different research groups, some mostly theoretical such as MIT LIDS (Laboratory for Information & Decision Systems) and other more systems-related groups, such as Charles Leiserson's SuperTech group that focuses on performance engineering research or MIT PDOS (Parallel and Distributed Operating Systems) group. UROP is usually a low to medium level commitment for students one semester at a time, and students often do UROPs only for a semester / change UROPs between semesters. Make sure to find a UROP that you really love, and if you don't like a UROP, try a different one. A good way to find UROPs is to look up the professors that teach classes you enjoyed. Note that UROPs are recommended but not required, and it is completely ok to be too busy to pursue a UROP during a particular semester.

For a more serious research experience, students can pursue a **SuperUROP**, which is just a UROP but for an entire year. **SuperUROPs** involve a poster presentation at the end of the year and involve some additional class work on top of a UROP. SuperUROPs can often lead to a master thesis.

## Internships

Like other universities, MIT supports its students to pursue internships during the summers. MIT also offers some additional benefits in this regard.

### Career Fair

Every fall, MIT hosts a Career Fair for all its students, but mostly geared for cs students. 

For freshmen and sophomore with little to no prior work experience, target small companies that aren't super competitive. Unless you know basic algorithms, you will probably not get an interview at companies like Google or Facebook initially, and even if you do get one, you would have to prepare quite a bit to be on par with other candidates. There are lots of small companies looking for interns that are willing to learn; you just have to find those companies as an underclassmen.

Juniors and seniors, Career Fair is a much more important for you. You may find the resume-defining internship or your first full-time job. Make sure you do your research beforehand and target companies that match your interests. 

When talking to recruiters, try asking questions about what the company does that isn't surface level information that anyone can find out by googling. Some questions that worked for me are

* What's a typical day at the company like, work-flow wise?
* I heard that the company recently (*insert recent events about company here*), how has that affected the company so far?
* I've heard that the company culture is collaborative, is there an experience at work that exemplifies this in your opinion? 

When it's your turn to tell them about yourself, go for short-and-sweet, but inviting, so that if recruiters want to know more, they will ask. Underclassmen will have to express their willingness to learn anything as opposed to pointint out past work and experience in related fields. These "recruiters" are often the software engineers that will conduct the actual interviews, so it may help more to talk about *what* you did instead of *where* you did it at. Read the body language; you can usually tell if a recruiter is excited about you or not. Regardless, drop a resume, since many companies email all resume a coding challenge as a first-round interview.

If recruiters like you, they will ask for your availability in the next 2-3 days if they are extremely interested in you. First-round interviews will be conducted on MIT campus for the next few days for lots of companies, and some interviews even happen minutes after Career Fair happens. There won't be a lot of time to practice coding questions once Career Fair happens, so any preparation in interview questions would have to happen way before Career Fair, likely during the summer. If recruiters like your interview, you will likely be invited to an onsite sometime in the coming months. Thus, for upperclassmen, most of fall is dedicated to flying all over the country for interviews.

### IAP / Externships / MISTI

MIT has a one month gap between fall and spring semesters called **IAP**, and MIT alumni use that opportunity to offer current students different work experiences. This proves to be a huge advantage, since most MIT students can accrue twice the amount of work and internship experience by the time they graduate compared to lots of typical universities nationwide.

Perhaps the most useful for cs students, MIT IAP offers an externship program. Students have to apply to the externship program in the fall. Externships are basically mini internships that still allow students to put company names on their resume, and many big name companies such as Google, IBM, Nasdaq, and Five Rings Capital all offer externships over the month of January.

To get an externship, students submit an application, and a recruiter will reach out if interested. Externship interviews vary; some are not technical, while others involve hard coding questions. For upperclassmen, the interview will likely be more about their interests rather than their technical ability, which their resume can usually attest to. Since each student can only apply up to 3 externships, **make sure to apply to companies that you are very interested in externing with, and ones that seem within reach given your current ability / resume**. 

Apart from externships, students can also pursue **MISTI** opportunities, which are subsidized opportunities to go abroad, usually to teach or work in a startup. MISTI happens over IAP as well as over the summer, and many students who already have internships over the summer use IAP to travel internationally through MISTI. While these do not directly help with cs, some MISTI programs are related to cs, such as **Middle-East Entrepreneurs of Tomorrow (MEET)**, where MIT students go to Israel to teach computer science to both Israeli and Palestinian kids. 

Lastly, MIT offers a lot of useful classes over IAP on campus for underclassmen, who are less likely to land externships and MISTI opportunities. Some of the most useful classes that significantly help cs careers are:
* **6.148 Web Programming Competition**. Basically teaches you how to build a functional, dynamic website. *Heavily* recommend.
* **MASLAB**. Robotics competition.
* **6.176 Pokerbots**. Computerized poker tournament. Lots of fun with algo, ml, and coding.
* **6.147 Battlecode Programming Competition**. AI coding contest in Java.

These are the most popular classes, and lots of other classes are offered during this time.

Students can also UROP over IAP.


## Other

Here are some other miscellanious things I found helpful:

* MIT Student Center's 5th floor makes for an amazing late-night studying spot.
* TA or LA a class as soon as you can. It's rewarding and helpful for (graduate) funding.
* Start labs / psets early, and try doing them by yourself first for optimal learning experience.
* Find good pset partners. Nothing brings people closer together like pulling all-nighters together.
* That said, don't pull all-nighters unless you have to. You'll know deep down if you have to.
* *Go to office hours, it will save you tons of time*.
* Use Piazza, it's your friend.
* Don't skip lectures that aren't recorded or ones that score in-class partipation.
* Talk to juniors and seniors about their general cs experience; they are goldmines.
* Being nice / having a good rep among MIT peers is more important than doing well in classes.
* *Please don't feel pressured to take 60 units a semester just b/c others do*.
* MIT is extremely difficult. You'll come out different. It's ok to ask for help, mental or academic.
* Don't skip meals.
* Shower.
* Don't spend *toooo* much time on MIT Confessions.


Cheers, and feel free to reach out if you have any questions!

*Thanks to [Brian Xie](http://www.brianxie.me/) for post feedback & [Bobbie Chen](https://bobbiechen.com/) for inspiration on making a tech blog.*