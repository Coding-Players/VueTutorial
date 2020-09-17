<template>
    <div class="Data_showing">
        <h1>{{ message }}</h1><br>
        <input type="text" v-model="message">
        <button>Save</button>
    </div>
</template>


<script>
export default {
    name: 'BasicDataTute',
    data(){
        return{
            message: 'Hi'
        }
    }
}
</script>

<style scoped>

.Data_showing{
    width: 100%;
    height: 200px;
    background-color: grey;
    color: #fff;
    text-align: center;
}
</style>