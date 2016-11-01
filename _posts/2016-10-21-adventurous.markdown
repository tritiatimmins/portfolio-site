---
layout: post
title:  "Adventurous"
---

## Adventurous is a travel app designed for mobile and web that allows users to save and upload points of interest in different locations around the world.

<div class="container">
  <h3>Project Overview</h3>
  <p>Adventurous was a project that I worked on with two other engineers while I was a student at Telegraph Academy. We had three weeks to create the app. At the time we were focused on functionality and paid little attention to visual design or user experience. In October I set out to revamp this project by adding to its visual design and creating mockups of new features that improve the user experience.</p>
</div>

<div class="container">
  <h3> Contributions</h3>
  <div class="title">
    <h4>Front-end engineer</h4>
    <ul>
      <li>Architected mobile routes</li>
      <li>Implemented UI in React-Native</li>
    </ul>
  </div>
  <div class="title">
    <h4>Scrum Master</h4>
    <ul>
      <li>Planned sprints to meet feature deadlines</li>
      <li>Made a list of standup etiquitte and communication guidelines</li>
    </ul>
  </div>
  <div class="title">
    <h4>Visual Design</h4>
    <ul>
      <li>Typography</li>
      <li>Color Scheme</li>
      <li>UI Design</li>
    </ul>
  </div>  
  <div class="title">
    <h4>UX Designer</h4>
    <ul>
      <li>Information Architecture</li>
      <li>Designed lo-fi Wireframes</li>
      <li>Created interactive prototype</li>
    </ul>
  </div>

</div>

<div class="container">
  <h2>BEFORE</h2>
    <p>Overall the process of adding a new point of interest to the map was very bare bones. A few things stuck out to me - a lack of options when it came to selecting photos and nothing telling you about what you just did.</p>
  <h3>Some immediate areas for improvement</h3>
  <ul>
    <li>Wouldn't it be nice if you could select existing photos from your photo library?</li>
    <li>Why does the icon selection symbol look like a warning icon?</li>
    <li>Let's come up with a way for users to know that they just added a post to the map and give them an option to edit it in the future</li>
  </ul>

    <img src="{{ site.baseurl }}/images/BEFORE.png" alt="Adventurous Mockup" height="500px">
  
  <h2>AFTER</h2>
    <p>In this series of wireframes I've outlined a flow of features that can solve the problems mentioned above.</p>
  <ul>
    <li>Users are also given the option of selecting an existing photo from their library. This gives them more flexibility.</li>
    <li>Adventurous only allows images that fit inside of the post editing area, so if a user wants to use an existing image they must crop it in order for it to fit.</li>
    <li>The icon to add an activity category was moved to the right side of the title input. This is so it looks more readable to the user. They can add their title, then select the category.</li>
    <li>Notifications were added to let the user know that their point of interest has been added to the map. Previously users only knew of this change by seeing an additional pin on the map.</li>
    <li>Another option is to add a glowing border around the new post for a few minutes after it has been created. This could be implemented using a setTimeout type of function.</li>
  </ul>

    <img src="{{ site.baseurl }}/images/userFlow.jpg" alt="Adventurous Mockup" height="500px">

</div>

<div class="container">
 <h3>Takeaways </h3>
 <ul>
    <li>When designing for mobile, we have to consider that the navigation thorugh the app is completely different than with a web app. In mobile, navigation is implemented through a stack. With each screen you add to the app, you add another item to the stack. This is important to remember especially when implementing functionality that allows you to go back to a previous screen.</li>
    <li>It is also important to remember that with mobile your space is limited. You must limit the amount of interactions you have per view. </li>
 </ul>
</div>

<div class="center">
  <ul class="actions">
    <li><a href="https://github.com/picnicsummit/biketrader" class="button big alt">See Adventurous on GitHub</a></li>
    <li><a href="{{ site.baseurl }}/portfolio.html" class="button big special">Checkout More of My Work</a></li>
  </ul>
</div>