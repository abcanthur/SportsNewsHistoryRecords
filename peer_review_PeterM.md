## Why?
- You will provide your peers with valuable feedback for their cornerstone project.
- You will receive said valuable feedback from **two** peers as well - making your cornerstone project that much better.
- You will gain insight into issues you might have on your own project.
- You will learn how to provide a semi-formal code review. Code reviews **will** be part of your job, its important to learn how they work.


## Guide to giving peer feedback

### Forking the project and preparation:
- 1. Fork your peer's repo into your github account.
- 2. Create a new ```peer_review.md``` file on **your peer project fork**. 
- 3. Copy the contents of **this** file and **paste** them into ```peer_review.md``` file you created on **your fork**.

### Creating peer review pull request:
- 1. Now you should be able to create a **pull request** from your fork back to your peer's original repo.
- 2. Title the pull request with: ```Peer review: Your Name```.
- 3. In the comments section, copy each question from below and answer it!

### Questions to answer:
##### 1. Does the project appear to meet the technical requirements? **Write up one sentence on your findings and give a score 0-3.**
- Is your peer making API calls, using SDK's/third-party libraries?
- Yes, it appears the sports news is all coming form the nytimes article search api
- Is your peer making use of Services? If so, are they offloading long tasks to a separate thread, i.e. AsyncTask, Runnable, IntentService, etc.
- no services defined. Retrofit query is automatically async
- Is your peer making use of Fragments? If so, are they passing data from Fragment to Activity via interfaces? If not, why did absense of Fragments make sense?
- Yes, fragments to organize the topics, leagues, news, records, etc
- Is your peer making use of RecyclerView? If so, does it appear to be working correctly ( implementation and otherwise )?
- Yes, recyclerViews are used for the AllSports, History, and League presentation
- Is your peer making use of some sort of persistent storage, i.e. Firebase or SQLite? If so, why do you think Firebase/SQLite was chosen? Could they have used one or the other instead and why?
- SQlite is used for the saveArticle feature. An excellent use!

##### 2. Does the project appear to be creative, innovative, and different from **any** competition? **Write up one sentence on your findings and give a score 0-3.**
- Is your peer making use of proper UX patterns we learned in class? If not, what are they doing that is unconvetional or that might confuse a user ( you )?
- Straightforward
- Is your peer making anything cool or awesome that you would like to note or applaud them on?
- Fish around for another api! There has to be some better sports sources than nyt. Hey, a spinner! nice 2.5/3

##### 3. Does the project appear to follow correct coding styles and best practices? **Write up one sentence on your findings and give a score 0-3.**
- Are you able to reasonably follow the code without having anyone answer your questions?
- note too well, lots of commented out chunks
- Are you able to make sense of what the code is doing or is trying to do?
- but yeah, I got the gist. It's mostly trying to parse nyt articles by league keywords 1.3/3

##### 4. Find two pieces of code of any size: one that is ```readable and easy to follow``` and one that is ```difficult to follow and understand```.
- What makes the readable code readable? **Be as detailed as you can in your answer, it can be challenging to explain why something is easy to undertand**
- What makes the difficult code harder to follow? **Be as detailed as you can in your answer**.
- mainActivity oncreate is jammed with a big switch statement (abstract this away) and two chunks of commented out code

##### 5. High level project overview: Take a look at as many individual files as you have time for
- Does this class make sense? 
- Does the structure of the class make sense?
- Is it clear what this class is supposed to do?
