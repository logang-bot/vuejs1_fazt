<template>
<div>
    <input type="text" v-on:keyup.enter="typing">
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
        },
        typing(e){
            console.log("dio un enter");
        }
    }
}
</script>

<style scoped>

</style>