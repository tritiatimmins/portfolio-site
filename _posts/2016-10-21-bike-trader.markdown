---
layout: post
title:  "Bike Trader"
date:   2016-10-21 17:30:44
---

Bike Trader is a web app that allows users to create a profile, view bicycle classifieds, sell bicycles, and view a list of Bay Area Cycling events. Bike Trader aims to not only create a hub of bicycle sales, but it also strives to create a community of cyclists and cycling enthusiasts.

<div class="center">

  <h3>Project Overview</h3>
  <p>I initially got the idea for Bike Trader while searching for bikes on Craigslist. My initial thought was wouldn't it be nice to have a one stop shop for buying used bikes that wasn't as anonymous as Craigslist? The idea for Bike Trader was born. When I was attending Telegraph Academy, I knew I'd like to try and turn this idea into an app. Bike Trader was a project I worked on with two engineers at Telegraph Academy. We had one week to create this app, starting on March 4th and finishing on March 13th. Like my other project, Adventurous, we were very focused on understanding the MEAN stack and making our app functional. Bike Trader was built using the MEAN Stack - Angular Js on the front end, Express and Node on the server side, and MongoDB for our database.</p>

  <h4>A UX Makeover (Still in Progress)</h4>
  <p>I love the idea of Bike Trader being a community for cyclists to connect with each other, so I wanted to revisit this project and rethink it from a user centered design perspective. So on October 21st, I decided to give it a UX makeover. I wanted to ask myself what kinds of features and styling could I add to make this product more enjoyable and easier to use? Althought this project is still in progress, I thought I would share what I have so far!</p>
</div>

<div class="container">

  <div class="center">
    <h3>Contributions</h3>

    <h4>UX Designer</h4>
    <ul>
      <li>Researched trends in Ecommerce and researched similar products</li>
      <li>Created Lo-Fidelity wireframes using Sketch</li>
      <li>Designed the information architecture of the classifieds section</li>
    </ul>

    <h4>Product Owner</h4>

    <p>To realize the product vision, I created a list of features I wanted to see in the app, and I presented these to the engineers. From there we collaborated on which features we thought fit the vision best and how feasible they would be to create. Then I prioritized the feature set and used that to define the MVP. After prioritizing the features I created wireframes of our product, and collaborated with our scrum master to plan sprint guidelines.</p>

    <h4>Full-Stack Engineer</h4>
    <ul>
      <li>Set up a factory in AngularJS to get information from our database</li>
      <li>Modeled a database schema using Mongoose a MongoDB ORM</li>
    </ul>

  </div>
</div>

<div class="center">
  <h2>Research</h2>
  <p>Before I dove in to creating wireframes and sketching, I did research on ecommerce applications and on products similar to Bike Trader.</p>

  <h4>E-Commerce Research</h4>
  <p>I chose to research e-commerce because a big part of Bike Trader is the bycicle classifieds ads. Although e-commerce and classifieds are slightly different, I feel that they are similar in that they facilitate the selling of goods. In order for Bike Trader to be a successful product, it would need to turn those classified ads into successful sales. Otherwise users would not want to use the platform.</p>
  <p>My research showed me that shoppers can be broadly put into two categories. There are "power shoppers" and there are casual browsers. "Power shoppers" tend to know exactly what they are looking for, and will find more descriptive ads and filters helpful because they are less likely to want to spend more time looking for what they want. On the other hand, browsers tend to have more time on their hands and don't need as much information when looking through items. This lead me to research integrating a 'list view' and a 'grid view' into the Bike Trader Classifieds. According to my research, list views can be more helpful for power shoppers and grid views can be more helpful for browsers. In addition, this feature can be helpful because there are those that process information more visually and others can obtain more information through more text-heavy views. </p>
  <p>I also did research into filters. Some of the sources I looked at advocated for putting filters on the left side. This way users could view their filters while being able to see the products change based on their selected criteria. However another source argued that it can be more helpful to add filters at the top of the page. Not only is this helpful for sites with infinite scrolling, but it is also helpful when creating a responsive design. For Bike Trader, I decided to go with a filter at the top because I want to maximize screen space.</p>

  <h4>Product Research</h4>
  <p>I evaluated three other products while doing research for Bike Trader. The first was Craigslist because Craigslist was a big inspiration for Bike Trader. The things I liked about Craigslist were it's display toggles between a list view and a grid view. That supported my ecommerce research and I definitely wanted to encorporate something like that into Bike Trader. However what I didn't like about Craigslist (although you could also argue this is what makes Craigslist so successful) was how anonymous it was. You had no idea who you were buying your bike from. Another thing I didn't think was helpful was that you couldn't refine your search for bikes based on things like size, year, or condition. These were things that I would like to see in a bicycle centric classifieds site like Bike Trader.</p>
  <p>The second product I looked at was Letgo, a new app that allows users to sell items much like Craigslist. What I liked about Letgo was that when you clicked on an item you could see a more detailed view of the product and you could also see a link to the user selling that item and other items they were selling. It attempts to solve the Craigslist anonymity issue. I also liked this idea because for Bike Trader it could help instill the sense of community that the product aims to create. If a user knows who buying their bike from, it helps the user feel like they belong to a community of other cyclists. I also looked at AirBnB because I think their product does a good job of creating a sense of trust between those renting out their houses and those looking for places to stay. That sense of trust is important for creating a community.</p>
</div>

<div class="center">
  <h2>WIREFRAMING</h2>
  <p>Here I have created low fidelity wireframes of the classifieds section of Bike Trader. The next step is going to be creating a prototype of my mockups to test the usability.</p>
  <img width="100%" src="{{site.baseurl}}/images/SearchingFiltering.svg" alt="Searching, filtering, and toggling between list and grid views"/>
  <img width="100%" src="{{site.baseurl}}/images/ListView.svg" alt="ListView"/>
  <img width="100%" src="{{site.baseurl}}/images/GridView.svg" alt="GridView"/>
  <img width="100%" src="{{site.baseurl}}/images/DetailedAdView.svg" alt="Detailed ad view"/>
</div>

<div class="center">
  <h2>NEXT STEPS - TESTING & VISUAL DESIGN</h2>
  <p>The next step will be designing a study and creating tasks. Then I want to remotely test the low fidelity wireframes on InVision and TryMyUI.</p>

  <p>I am also working on branding and visual design for Bike Trader. These are coming soon!</p>
</div>

<div class="center">
 <h3> Valuable Takeaways </h3>
</div>
<ul>
    <li>Researching E-commerce has been really helpful in shaping how I have determined the features and went about creating the wireframes.</li>
    <li>This project helped solidify my understanding of the MEAN stack and how all of the technologies come together to create a full stack application.</li>
    <li>I learned that collaboration with engineers is really important when defining your MVP or prioritizing features. Their previous experience with building similar features can give good insight into the time it might take to implement a particular feature.</li>
    <li>Clarity is key when defining features. You have to be able to communicate one thing in a few different ways because your interpretation of how a feature works may be completely different than how another person percieves that feature.</li>
    <li>Underestimating the complexity of a feature can be dangerous! I took on the challenge of figuring out how to upload images on the front end and store them on the backend. I thought it seemed relatively straightforward, but it turns out this process was much more complicated than I initially thought. I learned that it's important to do some investigation into how to implement a feature when you're in the feature prioritization phase of your project.</li>
 </ul>


<div class="center">
  <ul class="actions">
  <!-- button to view prototype on invision -->
<!--     <li><a href="{{ site.baseurl }}/portfolio.html" class="button big special">Checkout More of My Work</a></li> -->
    <li><a href="https://github.com/picnicsummit/biketrader" class="button big alt">See BikeTrader on GitHub</a></li>
  </ul>
</div>