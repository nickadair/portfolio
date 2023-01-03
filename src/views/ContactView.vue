<template>
  <div class="contact-info">    
    <a href="mailto:nick.adair@live.com">
      <i class="fa fa-envelope" />
      nick.adair@live.com
    </a>
  </div>
</template>

<style>
@media (min-width: 768px) {
  .about {
    min-height: 100vh;
    display: flex;
    align-items: center;
  }

  .contact-info {
    color: black;
    font-size: 2rem;
  }

  .contact-info a {
    color: black;
    text-decoration: none;
  }

  .contact-info a:hover {
    background-color: transparent;
    text-decoration: underline;
  }
}
</style>
