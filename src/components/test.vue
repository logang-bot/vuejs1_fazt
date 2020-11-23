<template>
<div>
    <input type="text" v-model="user.firstName">
    <button type="button" v-on:click="saludar(user.firstName)">
        CLICK ME
    </button>
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
        saludar(name ){
            alert("hello "+name)
        }
    }
}
</script>

<style scoped>

</style>