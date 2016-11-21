---
layout: post
title:  "Adventurous"
---
<p>Adventurous is a travel app designed for mobile and web that allows users to save and upload points of interest in different locations around the world.<p>
<div class="center"> 
  <img class="smallerImage" src="{{site.baseurl}}/images/MapView.svg" alt="Adventurous Map Screenshot"/>
  <img class="smallerImage" src="{{site.baseurl}}/images/EditPostFinishedGallery.png" alt="Adventurous Edit Post Screenshot"/>
  <img class="smallerImage" src="{{site.baseurl}}/images/CameraCapture.png" alt="Adventurous Campera Screenshot"/>
</div>

<div class="center">
  <h2>Project Overview</h2>
  <p>Adventurous was a capstone project that I worked on with two engineers while I was a student at Telegraph Academy. In three weeks we were able to work together to create a web and mobile app made with React and React Native. At the time we were focused on functionality and learning the new technologies, so we paid little attention to visual design or user experience.</p>

  <h2>UX Revamp</h2>
  <p>In late October, I decided to add to my UX skillset by improving the UX of one of my projects from Telegraph Academy called, Adventurous. For this project, I selected one of our features that I worked on as an engineer - Posting a new location to the map. I wanted to think of different ways that I could make this process more intuitive and give it more options to enrich the user experience.</p>
</div>

<div class="center">
  <h2> UX Contributions</h2>
  <div class="titleContainer">
    <div class="title">
      <h4>UX Designer</h4>
      <ul>
        <li>Evaluated existing product</li>
        <li>Identified areas for improvement</li>
        <li>Designed lo-fi Wireframes</li>
        <li>Created interactive prototype</li>
      </ul>
    </div>
    <div class="title">
      <h4>Visual Design</h4>
      <ul>
        <li>Evaluated existing UI</li>
        <li>Typography</li>
        <li>Color Scheme</li>
        <li>Redesigned UI</li>
      </ul>
    </div>
  </div>
  <h2>Engineering Contributions</h2>
  <div class="titleContainer">
    <div class="title">
      <h4>Front-end engineer</h4>
      <ul>
        <li>Architected mobile routes</li>
        <li>Implemented UI using React-Native</li>
        <li>Integrated a camera module</li>
        <li>Styled UI using Flexbox for responsiveness on different devices</li>
      </ul>
    </div>
    <div class="title">
      <h4>Scrum Master</h4>
      <ul>
        <li>Planned sprints to meet feature deadlines</li>
        <li>Held daily standups to discuss blockers, goals, and accomplishments</li>
        <li>Created guidelines for standup etiquitte and communication rules</li>
      </ul>
    </div>  
  </div>
</div>

<div class="center">
  <h2>BEFORE</h2>
</div>
<div>
  <p>Overall the process of adding a new point of interest to the map was very bare bones. A few things stuck out to me - a lack of options when it came to selecting photos and nothing telling you about what you just did.</p>
  
  <div class="imageContainer">
    <img class="centeredImage" src="{{ site.baseurl }}/images/BEFORE.png" alt="Adventurous Mockup">
  </div>

<div class="container">
  <div class="center">
    <h3>Areas for Improvement</h3>
  </div>
  <ol>
    <li>Some of the pins are the same color, but have different icons. Since each pin represents a different type of activity, unique activities should have a unique color and icon.</li>
    <li>The plus symbol in the middle of the add icon is too small. It should be larger, and a different color should be used. Green would be a more appropriate color because it is associated with exploration and security.</li>
    <li>The app only allows you to take pictures, but wouldn't it be nice if you could select existing photos from your phones gallery?</li>
    <li>What if you want to take a selfie or take a photo in low light conditions? Utilizing the iPhone's a flash and front facing camera would be an addition that solves this problem.</li>
    <li>Why does the category icon selection symbol look like a warning icon? The user would probably be confused and think they were seeing an error message. A more appropriate icon that symbolizes categorization would fix this problem.</li>
    <li>Putting the save button at the bottom is not consistent with the top navigation. If the user is able to go backwards with the navigation bar at the top, they will expect to use it to navigate forward. Using the word "save" is misleading. Is the user saving this activity to be posted later? Or are they going to share it now? Using a word like "share" or "done" would be more clear.</li>
    <li>Small nitpick, but there's no option for park! Hiking and garden are good options, but what about adding a park?</li>
    <li>The description has very small text for a large area of whitespace. The product owner wanted to see short, one to two sentence descriptions. Increasing the font size and reducing the size of the input can be helpful to reduce the amount of whitespace.</li>
    <li>Where's my new post? I want to create a way for users to know that they just added a post to the map and give them an option to edit it in the future.</li>
  </ol>
  
  <div class="center">
    <h2>WIREFRAMING</h2>
  </div>
    <p>In this series of low fidelity wireframes I've outlined a user flow of features that aim to solve the problems identified above.</p>
    
    <div class="imageContainer">
     <img id="myImg" class="centeredImage" src="{{ site.baseurl }}/images/newPointOfInterestFlow.png" alt="Adventurous Wireframe" height="500px">
    </div>

    <div id="myModal" class="modal">
      <!-- The Close Button -->
      <span class="close" onclick="document.getElementById('myModal').style.display='none'">X</span>

      <!-- Modal Content (The Image) -->
      <img class="modal-content" id="img01">

      <!-- Modal Caption (Image Text) -->
      <div id="caption"></div>
    </div>

<script>
   var modal = document.getElementById('myModal');

  // Get the image and insert it inside the modal - use its "alt" text as a caption
  var img = document.getElementById('myImg');
  var modalImg = document.getElementById("img01");
  var captionText = document.getElementById("caption");
  img.onclick = function(){
      modal.style.display = "block";
      modalImg.src = this.src;
      captionText.innerHTML = this.alt;
  }

// Get the <span> element that closes the modal
var span = document.getElementsByClassName("close")[0];

// When the user clicks on <span> (x), close the modal
span.onclick = function() { 
  modal.style.display = "none";
}
  </script>

  <ul>
    <li>An option for choosing the flash or front-facing camera was added.</li>
    <li>Users are also given the option of selecting an existing photo from their library. This gives them more flexibility.</li>
    <li>Adventurous only allows images that fit inside of the post editing area, so if a user wants to use an existing image they must crop it in order for it to fit.</li>
    <li>The icon to add an activity category was moved to the right side of the title input. This is so it looks more readable to the user. They can add their title, then select the category.</li>
    <li>Notifications were added to let the user know that their point of interest has been added to the map. Previously users only knew of this change by seeing an additional pin on the map.</li>
    <li>Another option is to add a glowing border around the new post for a few minutes after it has been created. This could be implemented using a setTimeout type of function.</li>
  </ul>
</div>

<div class="center">
  <h2>Prototyping</h2>
  <p>After I created the low fidelity mockups of how a user would add a new point to the map, I thought I would like to turn these wireframes into a medium fidelity interactive prototype.</p>
  <p>In the prototype mockups, I added color and typography to make the prototype look more realistic. You can check out the prototype <a target="_blank" href="https://projects.invisionapp.com/share/5496R2KFD#/screens/202123334_Map_View">here</a>!</p>
</div>

<!-- <div class="center">
  <h2>Visual Design - Typography & Color Scheme</h2>
  <p>I wanted to use a </p>
</div> -->

<div class="center">
 <h2>Takeaways </h2>
</div>
 <ul>
    <li>When designing for mobile, we have to consider that the navigation thorugh the app is completely different than with a web app. In mobile, navigation is implemented through a stack. With each screen you add to the app, you add another item to the stack. This is important to remember especially when implementing functionality that allows you to go back to a previous screen.</li>
    <li>It is also important to remember that with mobile your space is limited. You must limit the amount of interactions you have per view. </li>
 </ul>

<div class="center">
  <ul class="actions">
    <li><a href="https://github.com/picnicsummit/biketrader" class="button big alt">See Adventurous on GitHub</a></li>
  </ul>
</div>