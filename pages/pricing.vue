<template>
    <div>
        <div class="pricecards">
            <div>
                Element 1 <br> Price: {{price}}
            </div>
            <div>
                Element 2 <br> Price: {{price}}
            </div>
            <div>
                Element 3 <br> Price: {{price}}
            </div>
        </div>

        <ul class="uloverall">
            <li class="lioverall">
                <ul>
                    <li> Element 1</li>
                    <li> Price</li>
                </ul>
            </li>
            <li class="lioverall">
                <ul>
                    <li> Element 2</li>
                    <li> Price</li>
                </ul>
            </li>
            <li class="lioverall">
                <ul>
                    <li> Element 3</li>
                    <li> Price</li>
                </ul>
            </li>
        </ul>

    </div>
</template>

<script>
export default {
    data(){
        return{
            price:"$20"
        }
        
    }
}
</script>




<style scoped>
    .pricecards{
        background-color: rgba(115, 121, 119, 0.144);
        text-align: center;
        height: 800px;
        float: left;
        width: 100%;
        
        
    }

    .pricecards div{
        background-color:  #82ecd4;
        opacity: 0.8;
        width: 300px;
        height: 500px;
        position: relative;
        float: left;
        left: 25%;
        margin: 100px 0;
        font-size: 200%;
        transition-duration: 1s;

    }

      .pricecards div:hover{
        opacity: 1;
        width: 350px;
        height: 600px;   
    }

    .endfloat{
        float: none;
    }


    ul{
        list-style-type: none;
        padding: 0;
    }

    .uloverall{
        position: absolute;
        top: 900px;
        left: 25%;

        
    }

    .lioverall{
        float: left;
        text-align: center;
        background-color: #82ecd4;
        width: 300px;
        height: 500px;
        font-size: 200%;
        transition-duration: 1s;
        
    }

    .lioverall:hover{
        opacity: 1;
        width: 350px;
        height: 600px;   
    }
</style>