<template>
    <div class="users">
        <h1>user components</h1>
        <ul>
            <li v-for="user in users">
                {{user.name}} - {{user.email}}

            </li>
        </ul>

        <form v-on:submit="addUser">
            <input type="text" v-model="newUser.name" placeholder="nombre">
            <input type="email" v-model="newUser.email" placeholder="email">
            <button type="submit">
                Add
            </button>
        </form>
    </div>
</template>
<script>
export default {
    data(){
        return {
            users: [
                {
                    name: 'Joe',
                    email: 'joe@gmail.com',
                    contact: false
                },
                {
                    name: 'Ryan',
                    email: 'ryan@gmail.com',
                    contact: false
                },
                {
                    name: 'Miguel',
                    email: 'miguel@gmail.com',
                    contact: true
                }
            ],
            newUser: {}
        }
    },
    methods: {
        addUser(e){
            e.preventDefault();
            console.log("agregando usuario")
        }
    }
}
</script>
<style scoped>
    .users{
        background: #333;
        color: #fff;
        padding: 20px;
    }
</style>