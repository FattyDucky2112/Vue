<template>
    <div>
        <div :class="colorChange" class="container">
            <p :class="colorChange">This is the place to experiment with vue</p>
        </div>
        

        <div>
            {{message}}
            {{message2}}
            <br>
            {{emergencyText}}
        </div>
        <button @click="emergency = !emergency">{{emergencyText}}</button>
    </div>
</template>

<script>
export default {
    data(){
        return{
           message:"hello",
           message2:"world",
           emergency: true,
        }
    },
    computed: {

        emergencyText(){
            if(this.emergency){
                return "it is dangerous!!!!"
            }
            return "no danger"
        },

        colorChange(){
            if(this.emergency){
                return "colorchangeClass"
            }
        }

    }
}
</script>

<style scoped>
    .container{
        height: 60px;
        width: 50%;
        margin: 20px auto;
        text-align: center;
        left: 50%;
        border: 2px solid black;
    }

    .colorchangeClass{
        color: red;
        transform: rotate(10deg);
    }

</style>