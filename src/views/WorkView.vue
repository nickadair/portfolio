<script setup>
  import HexMenu from '../components/HexMenu.vue';
</script>

<template>
  <div class="worklist">
      <div class="light wide-tall">
        <img src="../assets/images/eekwi.org-old.jpeg" alt="" class="left">
        <div class="content">
          <h2>EEK Wisconsin</h2>
          <p>EEK Wisconsin is an environmental education site for kids. My part in the site was to convert the old static HTML site to a Drupal site with a more modern design. I worked closely with a designer to implement the front-end, and created the appropriate Drupal taxonomy and theme, including lots of custom functionality to give site content creators and editors an easy way to update the site, which at launch included several hundred articles and pages.</p>
          <a href="https://eekwi.org">EEK WI</a>
        </div>
        <img src="../assets/images/www.eekwi.org.jpeg" alt="" class="right">
      </div>
      <div class="dark wide-tall">
        <img src="../assets/images/www.tomahhealth.org-old.jpeg" alt="" class="left">
        <div class="content">
          <h2>Tomah Health</h2>
          <p>The Tomah Health site project was a redesign of the front page and updates to the Wordpress theme. The site design was created by a designer, and I implemented the changes to the Wordpress theme, including updates to the infrastructure and old plugins to ensure site security. The goals of the redesign were to simplify the content on the main page, but keep the primary calls to action that patients were already familiar with.</p>
          <a href="https://tomahhealth.org">Tomah Health</a>
        </div>
        <img src="../assets/images/www.tomahhealth.org.jpeg" alt="" class="right">
      </div>
      <div class="light wide-tall">
        <img src="../assets/images/neurology.wisc.edu-old.jpeg" alt="" class="left">
        <div class="content">
          <h2>Department of Neurology</h2>
          <p>The Neurology site was a total conversion of an old Drupal site using an outdated variation of the UW-Madison design. The goal was to move the site to Wordpress, and take advantage of the already created UW-Madison Wordpress theme. My part was to provision and manage the web server and associated tools such as database and caching server, move all content from Drupal to WP, and implement any additional functional changes to the UW-Madison theme, which I implemented as a child theme.</p>
          <a href="https://neurology.wisc.edu">Department of Neurology</a>
        </div>
        <img src="../assets/images/neurology.wisc.edu.jpeg" alt="" class="right">
      </div>
      <div class="dark wide-tall">        
        <img src="../assets/images/tripweather.jpeg" alt="" class="left">
        <div class="content">
          <h2>Trip Weather</h2>
          <p>Trip Weather is a personal project written in pure HTML and Javascript that allows someone to check weather conditions along a specific route between two points. I created it from scratch, since I was always checking the weather while traveling, and wanted an easier way to determine what the weather would be along my route, at the time that I would be passing through specific points. The site uses a logarithmic method to determine which points along the route to check the weather for, then queries the National Weather Service to determine the conditions at that point and time.</p>
          <a href="https://tripweather.co">Trip Weather</a>
        </div>        
      </div>
  </div> 
</template>

<style>
@media (min-width: 768px) {
  .about {
    min-height: 100vh;
    display: flex;
    align-items: center;
  }

  .light {
    background-color: darkgray;
    color: black;
  }

  .light a {
    color: black;
  }

  .dark {
    background-color: black;
    color: white;
  }

  .dark a {
    color: white;
  }

  .wide-tall {
    min-width: 90vw;
    width: 90vw;
    display: flex;
    justify-content: space-between;
    padding: 1rem 2rem;
    border-radius: 5px;
    margin-bottom: 1rem;
  }

  .wide-tall p, h2, a {
    padding: 1rem 2rem;
    text-decoration: none;
  }

  .wide-tall a:hover {   
    background-color: transparent;
    text-decoration: underline;
  }

  .wide-tall img {
    width: 20%;
    height: 20%;
  }

  .worklist {
    margin-top: 10rem;    
  }

  .right {
    margin-left: auto;
  }

  .left {
    margin-right: auto;
  }
}
</style>
