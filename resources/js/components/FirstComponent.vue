<template>
    <div class="m-4">
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
                    first_name: 'primera',
                    last_name: 'primer last name'
                }
            }
        },
       mounted(){
           this.$parent.persona1 = this.persona
       }
    }
</script>
