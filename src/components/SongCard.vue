<template>
    <div>
        <img :src="image" alt="">
        <h4>{{ name }}</h4>
        <h2>{{ trackTitle }}</h2> 
        <generic-button :key="name" :name="name"/>
    </div>
</template>

<script>
import GenericButton from "./GenericButton.vue";


    export default {
        
        name: 'SongCard',
        components: {
                'generic-button': GenericButton
        },
        props: {
            name: String,
            trackTitle: String,
            image: String,
            buttonFunction: {
                type: String,
                default: 'Add Song'
            },
            },
            data(){
                return{

                }
            },
            
            
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