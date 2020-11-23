<template>
<div>
     <div v-text="title"></div>
     <div v-if="showName">
        <p>{{user.firstName}}</p>
     </div>
     <div v-else>
         <p>no puedo mostrar nombre</p>
     </div>
     <hr>
     <ul>
         <li v-for="task in tasks">
             {{task.title}}

         </li>
     </ul>
</div>
</template>

<script>
export default {
    data(){
        return{
            title: 'holaaaaa',
            user: {
                firstName: 'Joe',
                lastName: 'Mcmillan'
            },
            myhtml: '<h3>hola vueee</h3>',
            showName: true,
            tasks: [
                {title: 'eat'},
                {title: 'dinner'}
            ]
        }
    },
    methods: {
        
    }
}
</script>

<style scoped>

</style>