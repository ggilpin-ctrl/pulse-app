# pulse-app
Capstone Project - Health and Wellness app

##Project Overview 
This project is of an app that will esssentially have everything oyu need all in one place. The main attraction to the app will have health apps where you can track workouts, what you eat, your activities etc. Also, there will some apps that will give you reminders and connect to your calendar, have mental health check ins. TOne of the main apps I would like to create is a workout app that will help with the use of AI by kniwng what the users goals are and help come up wiht weekly workout plans to help them acheive their goals. WIth all the wellness apps, I am going to have analytics that help track the indviduals doing, adn if they are active consistently they will get badges. 

##Project Phases
Phase 1 - Project Setup & Planning
Phase 2 - Design & Architecture
Phase 3 - Core Feature Development
Phase 4 - Testing and Refinement 
Phase 5 - FInalization adn Presentation

## Figma Design
Core feature UI designs are available here: https://www.figma.com/make/L4xdVprya2f9rGWY36SI9f/Pulse-App-Dashboard?t=jQWjzPvIq7KpPq0N-20&fullscreen=1 

## Project Log 
1/25/26: Respitory created adn intial README setup.

3/12/ 26: I just opened my read me file and nothing has saved.....


## Core Feauture
So the first thing I a going to create is the core feature. Essenjtially this will be a mood journal / daily check in system. I want this to be my core feauture becasue it has simple functions that will be easiet to learn. i think this is something that if I can get down then it iwll make the learning process easier for the other functions. I want to be able to get this fucntion down and then I can build other apps off of this one. This is a very fundamental app. 
This app will work by users will be able to quickly log their daily emotional state and then they have the option to quickly reflect on their day if they wanted too. This will also hopefull serve as the foundation for future analytics and mental wellness tracking within the app. 

## Development Process:
First I wanted to get an idea of exactly how I wanted this app to look. In my opionin, I think it iwll be easier to build if I know what the app looks like, and then i can go off of that.
So, I created a figma creation to help with the creation of what the app can look like. 

Here is the link to the figma file: https://www.figma.com/make/aKtjF8ju6YxyqkGzF2s4D7/Mood-journal-app-features?t=iCmOWyrMAsZYJ2J5-1

THe big thing for me was to make it visually appealing. I have the emoji centered in the middle of the screeen so users know to lcick it. ALso the colors are suppose to be very ncie to look at. The big thing fo rme and the hard part for this app will be the history tab. So that is righ tnext to wehre you can input the data. I will haev to do reserach in learning how to save entries thtough the coding. But I want it so that users can sewitch over to that button and tehn they can see all their history they have inputed on the days they have inputed data. 

First for the mood journal was to build the user interface using SwiftUI. SwiftUI allows the developer to build interfaces by stacking visual elements together. I used three main stacks such as Vstack Hstack and Zstack. A Vstack stacks elements vertically, a Hstack stacks elements horizonatlly, and a Zstack stacks elements on top of each other. So, I used the Zstack to create the background of the screen and place the main interface container on top of it. Inside that container I used a Vstack to organize the interfeace elements from to to bottom, such as teh title, mood selection, journal entry box, and save button.
For every mood button instead of writing seperate code for every mood button, I created a small list of moods that includes emoji, a label, and a value. Then I used a loop called ForEach to automatically generate a button for each mood in teh list. This made the code cleaner and easier to manage because if I ever want to add another mood, I only need to add it to the list rather than writing new button code.
Next, This made the code cleaner and easier to manage because if I ever want to add another mood, I only need to add it to the list rather than writing new button code.When the user clicks a mood button, the value of the selectedMood variable changes. SwiftUI automatically updates the interface when this happens. When the user clicks a mood button, the value of the selectedMood variable changes. SwiftUI automatically updates the interface when this happens.
For the jorunal entry box, I added a TextEditor component so users can write an optional journal note about their day. This text is stored in another state variable called journalText.
Them i createdsomething called a data model to represent each mood entry. A data model is simply a structure that defines what information should be stored. Each mood stores four peices of information. A unique ID so entries can be tracked , the mood emoji, the date the entry was created, and the optional jounral note. 

Once that was all done, i wasn't done with the entire mood app. But, I wanted to look what it teh visula of the screen looked like. The spacing of the mood journals were off. The boxes around the oods were not spcaed correctly. i was trying to fix my spacing and adjusting the width adn the spcae apart of each box. I was on this for awhile and it seemed like nothing would work. Finally, I figured out the boxes were just too big and make those smaller. That then fixed my problem. So there are teh grey boxes around each emoji. I wanted there to eb that white space between each of the grey boxes but also that space between the edge of the screen on the left and right of the end boxes. When i changed teh whole size of the grey boxes behind the emoji that seemed to fixed the visual problem I was having. 
Besides that the app seemed to look alright and function good.

2/14/26
** I got most of this app done on a six hour bus ride home from a basketball game. This is when I relazied I need to work on the app in long time periods. This is something that I have to sit down and focus on not a project that I can do periodically for like 30 minutes. So now I plan to do it once or twice a week and have like two hours of time that I am free to work on this project.


2/16/26
Now, it was time to do the history screen. This is the part where it switched to another tab. I was concerned that this would be hard to make. But to create this I had to create a second screen that displays previously saved mood entries. This screen uses a list of componet that automatically displays all entries stored in the mood history array. This was a whlel new tab on the left side panel. Calleed it HistoryView and the main file contentView calls it when the hisotry tab is clicked on. Each entry shows the mood emoji the date it was recorded, and the optional note. 

## 2/17/26 Bi-weekly checkin 
A biweekly checkin was due on 2/17/26. This was over our progress since last check in. Last check in I was a little behind. I should of had the app started, but till this check in, espacilly with the six hour bus ride I am all caught up. 
I plan to get this done before next check in: 
Implement persistent storage for mood entries (e.g., UserDefaults or local model
storage).
● Expand the MoodEntry data model if necessary.
● Improve the History view to display stored entries clearly.
● Add basic date formatting for saved entries.
● Conduct structured functional testing for entry creation and retrieval.

During this coding process I encountered many problems. A lot of it was really just getting an understanding a feel for the code. Since this is my first time really using SwiftUI code. Some things took me longer in the beginning because I have to research or remeber what function does what. And since I already know exactly what I wanted I had to find that function. But I think that knowing exactly what I wanted did help and make it easier to code. Also, another challenge I didnt't mention here but was something I just needed to figure out it works and connects within the app is how the @State works. 
Also, I have mentioned how I want my app to look a certain way. I have to start priortizing the functionality of my app rather than a clean good look interface. The interface took some time to do, but I think I just mainly wanted the interface to look clean for the first main core feature. Now it is time to start exp;anding the app, but now I have soemething I can start exoanding the app fucntionality rather than looks. And branching oof more files as it gets bigger. 
What I have learned- 
is through the time investment and when I am able to do this homework. I liek to do it when teh rest of my homework for the week is done. So I can soley focus on this. I spent a lot of time learning about how the code works and the variables of the code. Also, learned from an agile perspective the importance of adapting to plans when the intial timeline may seem off. 



2/23/26-
A big part was the saving data permantely. I created the app that took me like a week. 
