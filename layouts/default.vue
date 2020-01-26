<template>
  <div>
    <ul class="navlist">
      <li><nuxt-link to="/">Eintrag 1</nuxt-link></li>
      <li><nuxt-link to="/admin">Admin</nuxt-link></li>
    </ul>
    <nuxt />
  </div>
</template>

<style>
html {
  font-family: 'Source Sans Pro', -apple-system, BlinkMacSystemFont, 'Segoe UI',
    Roboto, 'Helvetica Neue', Arial, sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}

*,
*:before,
*:after {
  box-sizing: border-box;
  margin: 0;
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

.button--green {
  display: inline-block;
  border-radius: 4px;
  border: 1px solid #3b8070;
  color: #3b8070;
  text-decoration: none;
  padding: 10px 30px;
}

.button--green:hover {
  color: #fff;
  background-color: #3b8070;
}

.button--grey {
  display: inline-block;
  border-radius: 4px;
  border: 1px solid #35495e;
  color: #35495e;
  text-decoration: none;
  padding: 10px 30px;
  margin-left: 15px;
}

.button--grey:hover {
  color: #fff;
  background-color: #35495e;
}
</style>
