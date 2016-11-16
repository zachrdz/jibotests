# Jibo the Study Buddy

Jibo assisted interviewing for potential candidates to review material and be better prepared for their actual interview. They can interact with Jibo throughout the review process and use their results to assist them in getting the job they desire.

## Demo
[Video of Jibo simulator in action running our project.](https://youtu.be/hLXrqcb00Mg)

## Devpost
[Link to our Devpost submission for MLH Prime Southwest Regional](https://devpost.com/software/jibotests)

## Team Members
* Samantha Campos
* Zachary J. Rodriguez

## Inspiration
Our project takes aim at helping anyone searching for a job or even just studying for an upcoming test or certification. We know how tedious the process of reviewing material can be, as well as how boring it can be staring at a computer screen for hours hoping to remember the material you need to know. With Jibo, you can have someone to study with who basically knows everything you need to know.

## What it does
Jibo acts as a study buddy/interviewer who allows you to be interviewed on any topic you wish. Yes, you read that right, any topic! We leverage api's that give us access to a huge set of test banks and interview questions on any topic you can think of, that way when you ask Jibo to interview you on something, he'll be ready to fire back a great set of questions to get you ready for your next interview or exam. Once you're done with the set of questions, you'll get your results on how you did, as well as an email sent to you with the results and a link to a flash card set of the questions you were ask, so you can take your studying mobile!

## How we built it
We used the Jibo SDK, as well as used Quizlet's API for when querying for questions for a topic a user may ask to be interviewed on.

## Common Questions
* Are the questions that Jibo asks static and hard coded?
    * No, Jibo pull it's questions and answers dynamically for any topic you'd like to study. It does this by using API's to get that information.
* Can I have Jibo ask me a particular set of questions I'd like to study?
    * Yes! You can do this really easily. We leverage Quizlet's API for our questions. You can go to Quizlet's website, write out a study deck and save it, then ask Jibo to interview you on the name of the study deck you posted to Quizlet, and now jibo will ask you everything in that study deck and cross check your answers with the one's you provided. It's that easy!

## Challenges we ran into
Comparing answers given to the answers we had from our data source. Using Natural Language Processing that's built into Jibo, we were able to match the given answer with the expected answer with great accuracy.  Also, getting Jibo to react to your responses with fun and humorous responses of his own was a challenge, but we created some nice animations and sayings for him we think you'll enjoy. 

## Accomplishments that we're proud of
* Pulling our question set from Quizlet, so we are able to help you study practically anything
* Adding great animations and sayings for Jibo to use to interact with you
* Incorporating real time feed back as well as a results summary that we're able to email you with
* Understanding behavior trees and being able to understand the Jibo SDK in a short length of time

## What we learned
NodeJS, Behavior Trees, Jibo SDK

## What's next for JiboTests
Incorporate video recording to record your interaction with Jibo when being interviewed, to possibly send that along with your results when we communicate back to you via email and storing the video using storage api's. This would be useful for companies wanting to use the device as an interview tool, so they may see how a potential candidate answered the questions by reviewing the results along with the video. Also, adding more analytics on the results from the test to be able to suggest training material to the user as well as possible job positions they may be interested in based on the topics they are asking Jibo to interview them on and how well they do on these mock interviews.

## Built With
JiboSDK, NodeJS, Javascript, HTML, Quizlet API

## Developer Notes
Current queries for interview topics are limited to the following for demo purposes only.
* SQL (Must say "sequel")
* Data structures
* Object oriented programming
* Java

To enable unrestricted queries, please adjust the code in the .bt file to remove the filter/restriction.
You will then be able to query/be interviewed on any topic you say.

### Startup Commands
* "hey jibo"
* "interview me"
* "yes"

### Question Response Commands
* "skip" or "pass" (Skips to the next question)
* "tell me the answer" (Gives you the answer to the current question)
* "repeat" (Repeats the question to you)
* "correct answer given" (Makes your answer correct, usefuel when NLP matching isn't accurate enough)
