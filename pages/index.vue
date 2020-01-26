<template>
  <div class="jumbotron">

    <Logo message="abababab" />

    <div class="div1">
      hello index {{ light }}

          <img v-if="light" src="~assets/lighton.png">
          <img v-else src="~assets/lightoff.png">

    </div>
    <div>
      <button id="test" class=" btn btn-danger button" @click="light = !light">{{ buttonText }}</button>
    </div>
    

    <input type="text" v-model="message" @blur="validateInput">

    {{ message }}

  </div>
</template>

<style scoped>
  .div1{
    height: 50vh; 
    width: 100vh;
    overflow: hidden;
  }

  .div1 img {
    height: 60%;
  }
  
  .button {
    transition: all 1s ease;
    opacity: 0.5;
  }

  .button:hover {
    color: rgb(255, 255, 255);
    background-color: #ff0000;
    /* transform: rotate(-360deg); */
    opacity: 1;
  }
</style>


<script>
import Logo from '~/components/Logo'

export default {
  components: {
    Logo
  },
  data() {
    return {
      light: false,
      message: ''
    }
  },
  computed: {

    buttonText() {

      if (this.light) {
        return 'Switch off'
      }

      return 'Switch on'

    }

  },
  methods: {

    validateInput() {
      
      console.log(/[A-z]/.test(this.message))

    }
  },
  mounted() {



  }
}

</script>