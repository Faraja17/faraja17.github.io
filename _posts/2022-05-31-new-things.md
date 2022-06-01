## New Things


### Keeping organized with a custom Google Sheets app.

Frequently, an idea for a new system, invention, coding project, or blog post will come to me at a time when I am in the middle of a task. Rather than risking forgetting the idea by waiting for a more convenient time to jot it down in a designated notebook, or to type it into an organized list on the computer, I usually grab the nearest writing tools--could be a notepad and pencil, or even the back of a receipt or napkin and a Sharpie marker. Very quickly, these little slips of paper become lost or difficult to sift through. In today’s blog post, I describe the latest Google form/sheet “app” that I designed for my phone to help me keep organized. As I learn more and more about coding, I hope to one day use my “big girl tools” (Node.js, React, Json, Swift, etc.) to create real working web and phone apps, but for now, my love affair with Google Sheets continues because I can get quick results.


## Table of contents


- [Overview: Keeping Organized with a Custom Google Sheets App.](#keeping-organized-with-a-custom-google-sheets-app)
- [Park Ranger to Techie](#park-ranger-to-techie)
- [My New Ideas App Design](#my-new-ideas-app-design)
  - [Screenshots](#screenshots)
- [Installing the App and Future Projects](#installing-the-app-and-future-projects)
- [Closing](#closing)


### Park ranger to techie

First, a fun fact about me: I have served as a seasonal U.S. Park Ranger. Duing four years worth of summers and weekends, I had the dream job of demonstrating how hundred-year-old phonographs and cylinder records still play today as clear and beautiful as the day they were manufactured in Thomas Edison’s West Orange, New Jersey laboratory complex. I spent delightful hours exploring and researching, between giving tours of Glenmont, Edison’s opulent 29-room mansion in Llewellyn Park, a short drive away from the lab. Several of my own home’s furniture pieces and focal points have been inspired by what I beheld at Glenmont.


I have also been inspired by Edison’s work as an inventor, and his approaches to organizing over eighty years of ideas throughout his lifetime.  He jotted notes and drew sketches on loose pieces of paper, in pocket notebooks, and beginning in 1878, in formalized laboratory books—altogether, over five million pages of various notes! [You can read more about Edison and his papers here.](https://edison.rutgers.edu/about/thomas-edison-and-his-papers) 


Back at the lab, within a grand library designed by the same architect who had built Glenmont, resides Edison’s office desk on display. What is most amazing to me, about both the house and the lab, is the fact that *everything* within is original—no replicas. Edison’s desk was locked after his death in 1931. Since the desk was reopened in 1947, very little has changed. A particular cubby hole, labeled “New Things” continues to captivate me along with numerous other park visitors. It was where Edison kept his random scraps of paper, filled with ideas for new inventions.


### My new ideas app design

So, my problem is apparently common among creative types. However, Edison did not have access to a tiny computer to carry around with him everywhere, like I do. Over the years, I have already designed my own grocery list and house-hunting phone “apps” using Google Forms and Google Sheets. Recently, I designed an app that I call “New Ideas: My place to dump all my coding ideas.”  


I designed the app by first creating a Google Form with four prompts: *Project Name, Project Description, Blog Idea, and Blog Idea Descritption*.  Next, I clicked the Google Sheet icon at the top right. This generated a Google Sheet with the same title as the form to collect the form’s responses. The next step was to organize the responses in the Google Sheet.  This is where things became tricky.


Even though I was using the same form to collect both project and blog ideas, I wanted to be able to view them separately. So, at the bottom of the spreadsheet file, I created two additional tabs, one named *Personal Project Ideas* and the other *Blog Ideas*.  The tricky part was duplicating the data from the original *Form Responses* tab to populate and update into the two new tabs.  After a lot of searching online, and finally figuring out the keywords that would return my desired results, I located [a thread that helped](https://support.google.com/docs/thread/3884038/how-to-make-a-duplicate-column-in-that-will-continue-to-update-as-the-original-gets-new-data?hl=en).  After a bit of tweaking to fit my particular needs, I entered the following formula into each cell of the two tabs I’d created, and I was able to achieve my goal!


```

=filter('Form Responses 2'!B1:C,'Form Responses 2'!B1:B<>"")

```


Now, when I enter project and blog idea data using the Google Form, it is all automatically placed on the original *Form Responses* tab along with a time and date stamp. Then the project name and the description data are called by the formula and organized into two columns on the *Personal Project Ideas* tab.  The blog data is called and organized, in the same way, to the *Blog Ideas* tab.

#### Screenshots
Click images for fullscreen view.

| <b> </b>                                              |                                                                 |
|:---------------------------------------------------------------:|:---------------------------------------------------------------:|
|Form                                                             |Original Tab                                                                 |
| [![screenshot of Google Form](https://github.com/Faraja17/faraja17.github.io/blob/main/form.png?raw=true)](https://github.com/Faraja17/faraja17.github.io/blob/main/form.png?raw=true) | [![Screenshot of original Google Sheet Tab](https://github.com/Faraja17/faraja17.github.io/blob/main/original%20tab.png?raw=true)](https://github.com/Faraja17/faraja17.github.io/blob/main/original%20tab.png?raw=true) |


| <b> </b>                                             |                                                                 |
|:---------------------------------------------------------------:|:---------------------------------------------------------------:|
|Projects Tab                                                     |Blog Tab                                                                 |
| [![Screenshot of project ideas tab](https://github.com/Faraja17/faraja17.github.io/blob/main/projects%20tab.png?raw=true)](https://github.com/Faraja17/faraja17.github.io/blob/main/projects%20tab.png?raw=true) | [![screenshot of blog ideas tab](https://github.com/Faraja17/faraja17.github.io/blob/main/blog%20tab.png?raw=true)](https://github.com/Faraja17/faraja17.github.io/blob/main/blog%20tab.png?raw=true) |


### Installing the app and future projects 

In order to install the completed app, I navigated to the form through Google Drive on my (Android) phone, copied the URL. After opening the form through my phone’s Chrome web browser, I tapped the three dots on the upper right to access the browser menu, and tapped “Add to Home Screen”. This creates a labeled app-like link using the web page's favicon. Finally, I placed the app in its desired location on my home screen. I later decided to add a link to the response Google Sheet alongside it so that I can easily view my ideas as well. Now that I am becoming more comfortable writing in JavaScript, I am excited in the future to create my own [custom functions in Google Sheets using the Google Script Editor (YouTube video)](https://www.youtube.com/watch?v=DRmWYChhhLk). 

[![screenshot of apps on phone](https://github.com/Faraja17/faraja17.github.io/blob/main/image%20of%20apps.jpg?raw=true)](https://github.com/Faraja17/faraja17.github.io/blob/main/image%20of%20apps.jpg?raw=true)

### Closing

At the Thomas Edison National Historical Park, some of the rangers love to point out how the modern cellular phone represents Edison’s work in light, sound, video, and storage batteries.  I’m sure he would have marveled at all of its capabilities, and I like to imagine that he would have appreciated my little *New Ideas* app, too!

[![pic of me in my green and grey with niece and nephew at TENHP](https://github.com/Faraja17/faraja17.github.io/blob/main/Screen%20Shot%202022-06-01%20at%202.10.52%20AM.png?raw=true)](https://github.com/Faraja17/faraja17.github.io/blob/main/Screen%20Shot%202022-06-01%20at%202.10.52%20AM.png?raw=true)
