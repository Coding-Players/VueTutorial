<template>
    <div>
        <h2 v-if="show">{{ data }}</h2>
        <h2 v-else>It is else Statement in vue app</h2>
        <button v-on:click="display" >Toggle Different Data</button>
    </div>
</template>
<script>
export default {
    name: 'ConditionTute',
    props:{
        data:String
    },data(){
        return {show:true}
    },
    methods:{
        display(){
            this.show =! this.show
        }
    }
}
</script>
