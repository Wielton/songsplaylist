<template>
    
        <button>
    
    </button>
    
</template>

<script>
    export default {
        name: 'GenericButton',
        
        props: {
            name: String,
            
            
        },
        data() {
            return {}
        },
        methods: {
            buttonClicked() {
                this.$emit('buttonClicked', this.name);
                console.log('You clicked the button');
            }
        }
    }
</script>

<style scoped>
    
</style>