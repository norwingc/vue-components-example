<template>
    <div class="container">
        <first-component></first-component>
        <second-component></second-component>
        <button @click="save">Save</button>
        <br>
        <pre class="m-5">{{ persona1 }}</pre>
        <pre class="m-5">{{ persona2 }}</pre>
    </div>
</template>

<script>
import FirstComponent from './components/FirstComponent.vue'
import SecondComponent from './components/SecondComponent.vue'

export default {
    components:{
        'first-component' : FirstComponent,
        'second-component' : SecondComponent
    },
    data(){
        return{
            persona1: {},
            persona2: {}
        }
    },
    methods:{
        save(){
            cosole.log('fasdf')
        }
    }
}
</script>
