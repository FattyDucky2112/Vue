<template>
    <div>
        <p>{{event}}</p>
        <div class="grid-container">
            <ul v-for="item in items" class="grid-item">
                <li><img src="~assets/party.png" alt="Picture"></li>
                <li>{{item.event}}</li>
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
               items:[
                   {event:"Parteyyy1"},
                   {event:"Parteyyy2"},
                   {event:"Parteyyy3"},
                   {event:"Parteyyy4"},
                   {event:"Parteyyy5"},
               ]
            }

            
        }
}
</script>