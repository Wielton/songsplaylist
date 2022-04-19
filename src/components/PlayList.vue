<template>
    <div>
        <h1>Playlist</h1>
        <ul>
            <li></li>
        </ul>
    </div>
</template>

<script>

    export default {
        name: 'PlayList',
        components: {
            

        },
        data(){
            return{
                playList: [],
                
            }
        },
        props: {
            name: String,
            trackTitle: String,
            image: String
        }
    }
</script>

<style scoped>

</style>