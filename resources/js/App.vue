<template>
    <div class="container">
        <first-component v-on:childToParent="getDataOne" ref="childComponent"></first-component>
        <button @click="save">Save</button>
        <br>
        <pre class="m-5">{{ persona }}</pre>
    </div>
</template>

<script>
import FirstComponent from './components/FirstComponent.vue'

export default {
    components:{
        'first-component' : FirstComponent
    },
    data(){
        return{
            persona: {}
        }
    },
    methods:{
        getDataOne (value){
            this.persona = value
        },
        save(){
            console.log('fasdf')
        }
    },
    mounted(){
        this.$refs.childComponent.sendData()
    }
}
</script>
