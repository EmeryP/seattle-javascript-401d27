![cf](http://i.imgur.com/7v5ASc8.png) Facilitators Guide: Component Based UI
============================================================================
<a name="top"></a>

## Preparation
* Its React time, so get comfortable in the ecosystem.
* Students will really struggle on how things fit, what calls what, and how the magic works. Make sure that your demos and coding style leaves room for the rabbit holes, questions, and confusion that will arise.

## Lecture Main Topics & Overall Flow
* Take a walk down memory lane ...
  * Build the Vanilla demo
    * Talk pros and cons (ids, event listeners, difficult to change behavior, etc)
  * Build a jQuery demo
    * Pros and Cons - cleaner syntax, Handlebars takes a state and can be easily rendered without touching each thing.
    * Still hard to make sense of all the code
  * Build again in React
    * Sell the magic of "simply changing state to get a re-render"
    * Sell how little JS you actually had to write to make it happen
    * Sell how cool it was to make and render 3 components as "Markup"
* Break
* Now that it's simmered for a bit, lets jump into what happened there
  * Components
    * Header = <Header />, etc
      * Just like calling Header() from in a JS function, but easier
  * State
    * setState() does some event triggering behind the scenes for you
    * The app knows state and what bits care about it, and re-renders as it changes
    * You can focus on:
      * Building the parts and what things do given different "States"
      * What causes a state change
      * How to change state when that thing happens



## Live Coding Demo(s)
We'll be starting the day with creating the same application in 3 ways.
* Render the current state of the "counter" and "words"
* When a user changes an input field, update words and re-render
* On a button click, update the counter and re-render

#### Vanilla JS -- `demo-vanilla`
* Do the above in vanilla JS with event listeners

#### jQuery and Handlebars -- `demo-jquery-hb`
* Swap out the vanilla event listeners for jQuery equivalents
* Bring in handlebars to do a better job of rendering

#### React -- `demo-react`
* Write it in react, with a combination of functional and class components
* Talk through (briefly) setState and magical re-rendering

## Lab Prep
* The part of the lab assignment is to draw a process diagram of the starter code and state as events happen. Once the students understand that, they can move on.
* The "Work" part of lab is all about tinkering with the starter code. They will be converting to and between functional and class based components, putting them into different files, doing different things with state, etc. There's a lot of checkpoints along the way, but their final submission should resemble the solution code.
* Make sure and go through all the steps yourself so that you know the steps. Don't jump immediately to the solution, or you'll not be able to assist students as they plod through the practice exercises.
* Once all of the coding exercises are complete, the students should re-draw the process diagram to assert any changes based on how they broke things up and to ensure that state is being managed the same way.

## What bugs, issues, or surprises have come up in the past for this class?
* Understanding how things connect is always a tough nut for the students to crack.

## General Comments and Notes
*
