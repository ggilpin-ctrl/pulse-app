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
