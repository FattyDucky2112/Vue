

<template>
    <div>

        <div class="background">
            <div class="backgroundtext">
                <p>This is Thunder!</p>
            </div>
        </div>

        <div class="container">
            <label for="Username">Username</label>
            <input type="text" name="Username" id="" placeholder="type here">

            <label for="Story">Story</label>
            <input type="text" name="Story" id="" placeholder="funny story please">
        </div>
        <div class="container">
            <p>my name is: {{myname}}</p>
            <p>my name in reverse: {{reversedName}}</p>
         

        </div>
    </div>
</template>

<script>
    export default {
    data() {
        return {
        myname: 'Marco',
        }
    },
    computed: {

        reversedName() {
                return this.myname.split('').reverse().join('')
            },

        }
    }

</script>

<style scoped>
    p{
        margin: 0;
    }
    .container{
        margin: 20px auto;
        width: 50%;
        text-align: center;
        background-color: rgba(156, 144, 144, 0.171);
    }

    .container input{
        margin: 20px 5px;
    }

    .background{
        height: 500px;
        background-image: url("~assets/thunder.jpg");
        background-position: center;
        background-repeat: no-repeat;
        background-size: cover;
        opacity: 0.3;
    }

    .background:hover{
            opacity: 1;
        }
    
    .backgroundtext{
        text-align: center;
        position: relative;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
        color: white;
        font-size: 10rem;
        margin: 0;
    }

  
</style>

