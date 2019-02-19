<template>
    <div class="container">
        <first-component v-on:childToParent="getDataOne"></first-component>
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
            }
        }
}
</script>
