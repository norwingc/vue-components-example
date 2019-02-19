<template>
    <div class="m-5">
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Consectetur voluptatem delectus voluptate sit debitis consequuntur, similique, labore rem molestiae autem aspernatur quasi ad quod ipsa rerum nesciunt, tenetur maxime? Sunt!</p>
        <input type="text" v-model="persona.first_name">
        <input type="text" v-model="persona.last_name">
    </div>
</template>

<script>
    export default {
        data(){
            return{
                persona:{
                    first_name: 'segunda',
                    last_name: 'segunda last name'
                }
            }
        },
       mounted(){
           this.$parent.persona2 = this.persona
       }
    }
</script>

