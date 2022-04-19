<template>
    <div>
        
                <img :src="image" alt="">
                <h4>{{ name }}</h4>
                <h2>{{ trackTitle }}</h2> 
                <button @click="buttonClicked">{{buttonFunction}}</button>
            
    </div>
</template>

<script>



    export default {
        
        name: 'SongCard',
        components: {
                
        },
        props: {
                name: String,
                trackTitle: String,
                image: String,
                isSaved: Boolean,
                buttonClicked: Function,
                buttonFunction: {
                    type: String,
                    default: 'Click',
                    
                }
        },
            data(){
                return{

                }
            },
            methods: {
                
            
    }   
            
            }

</script>

<style scoped>
    div{
        box-sizing: border-box;
        border: none;
        box-shadow: 1px 2px 2px #383838;
        height: 300px;
        width: 500px;
    }
    img{
        width: 100px;
        height: 100px;
    }
</style>