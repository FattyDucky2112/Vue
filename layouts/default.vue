<template>
  <div>
    <ul class="navlist">
      <li><nuxt-link to="/home">Home</nuxt-link></li>
      <li><nuxt-link to="/admin">Admin</nuxt-link></li>
      <li><nuxt-link to="/fun">Fun</nuxt-link></li>
      <li><nuxt-link to="/pricing">Pricing</nuxt-link></li>
      <li><nuxt-link to="/events">Events</nuxt-link></li>
    </ul>
    <nuxt />
  </div>
</template>

<style>
@import url('https://fonts.googleapis.com/css?family=Sigmar+One&display=swap');
html, body {
  font-family: 'Sigmar One', cursive;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}

.navlist{
  list-style-type: none;
  margin: 0;
  padding: 0;
  height: 60px;
  background-color: #82ecd4;
  opacity: 0.6;
}

.navlist li{
  font-family: 'Sigmar One', cursive;
  float: left;
  background-color: #82ecd4;
  height: 100%;
  opacity: 0.6;
}

.navlist li:hover{
  float: left;
  background-color: #82ecd4;
  height: 100%;
  opacity: 1; 
}

.navlist li a{
  display: block;
  color: rgb(0, 0, 0);
  text-align: center;
  padding: 14px 16px;
  text-decoration: none;
  font-size: 20px;
}
</style>
