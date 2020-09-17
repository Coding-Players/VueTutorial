<template>
    <div>
        <h1>My Vue App Home Page.</h1>
        <h2> {{ data }}</h2>
        <button v-on:click="clickme" >click to alert</button>
        <button v-on:mouseover="datasender('From this button we send this data.')" >Data Send from here</button>
    </div>
</template>
<script>
export default {
    name: 'Home',
    props:{
        data:String
    }, 
    methods:{
        clickme(){
            // console.log('clicked')
            alert('clicked')
        },
        datasender(data){
            alert(data)
        }

    }
}
</script>
