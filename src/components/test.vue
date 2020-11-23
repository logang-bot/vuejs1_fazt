<template>
<div class="test">
    {{msg}}
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
    },
    computed: {
        fullName(){
            return this.user.firstName + ' ' + this.user.lastName
        }
    },
    props: {
        msg: {
            type: String
        }
    }
}
</script>

<style scoped>
    .test{
        background-color: #eee;
    }
</style>