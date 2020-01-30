<template>
    <div>
        <p>{{event}}</p>
        <div class="grid-container">
            <ul v-for="item in items" class="grid-item">
                <li><img src="~assets/party.png" alt="Picture"></li>
                <li>{{item}}</li>
            </ul>

            <!-- <ul class="grid-item">
                <li><img src="~assets/party.png" alt="Picture"></li>
                <li>{{event}}</li>
            </ul>
             <ul class="grid-item">
                <li><img src="~assets/party.png" alt="Picture"></li>
                <li>{{event}}</li>
            </ul>
              <ul class="grid-item">
                <li><img src="~assets/party.png" alt="Picture"></li>
                <li>{{event}}</li>
            </ul> -->
        </div>


    </div>
    



</template>

<style scoped>
    ul{
        list-style-type: none;
        padding: 0;
    }

    .grid-container{
        display: grid;
        grid-template-columns: auto auto auto;
        padding: 10px;
    }

    .grid-item{
        background-color: rgba(255, 255, 255, 0.8);
        padding: 20px;
        font-size: 30px;
        text-align: center;
        transition-duration: 1s;
        margin:0;
        max-width: 900px;
    }

     .grid-item:hover{
       box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);
    }
</style>

<script>
export default {

        data(){
            return{
                    items: ["Party1","Party2","Party3","Party4","Party5","Party6"]
                    
                // var: vegetable = class whatever { 
                //     constructor(name, link){
                //         this.name = name;
                //         this.link = link;
                //     }
                
                //  },
                // var: cabbage = new vegetable('cabbage', 'link'),

                // items:[cabbage]       
              
            }    
        }
}
</script>