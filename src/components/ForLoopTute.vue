<template>
    <div>
        <h2>{{ msg }}</h2>
        <div id="table_container">
            <table border="1px">
                <tr>
                    <td>Id</td>
                    <td>Name</td>
                    <td>Email</td>
                </tr>
                <tr v-for="user in users" :key="user.id">
                    <td>{{ user.id }}</td>
                    <td>{{ user.name }}</td>
                    <td>{{ user.email }}</td>
                </tr>
            </table>
        </div>
    </div>
</template>
<script>
export default {
    naem:'ForLoopTute',
    props:{
        msg:String
    }, data(){
        return {
            users: [
                {id:1, name: 'Sudipta', email: 'sudipta@gamil.com'},
                {id:2, name: 'Soumen', email: 'soumen@gamil.com'},
                {id:3, name: 'Pranay', email: 'pranay@gamil.com'},
                {id:4, name: 'Tanmay', email: 'tanmay@gamil.com'},
                {id:5, name: 'Madan', email: 'madan@gamil.com'},
                {id:6, name: 'Subhas', email: 'subhas@gamil.com'},
                {id:7, name: 'Prakash', email: 'prakash@gamil.com'},
            ]
        }
    }
}
</script>

<style>
#table_container {
    position: relative;
    background: #c1f9fd;
    color: green;
    display: flex;
    width: 100%;
    align-items: center;
    justify-content: center;
}
</style>