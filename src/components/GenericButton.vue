<template>
    
        <button @click="buttonClicked">
    {{buttonFunction}}
    </button>
    
</template>

<script>
    export default {
        name: 'GenericButton',
        
        props: {
            buttonFunction: String,
            name: String
            
        },
        data() {
            return {}
        },
        methods: {
            buttonClicked() {
                this.$emit('button-clicked')
            }
        }
    }
</script>

<style scoped>

</style>