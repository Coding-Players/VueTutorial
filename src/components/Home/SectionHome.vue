<template>
    <section>
        <div class="RandomText">
        <button v-bind:style="{backgroundColor:'gray', color: 'white'}">This is section Container</button><br>
        <button v-bind:class="{display:show}">This is section Container</button><br>
        <button v-bind:class="[aClass]">This is section Container</button><br>
        <button v-bind:class="[shown? 'yesShow':'noShow']">This is section Container</button><br>
        <button v-bind:style="{backgroundColor: bacColor}">This is section Container</button><br>
        <BasicDataTute/>


            For though result and talent add are parish valley. Songs in oh other avoid it hours woman style. In myself family as if be agreed. Gay collected son him knowledge delivered put. Added would end ask sight and asked saw dried house. Property expenses yourself occasion endeavor two may judgment she. Me of soon rank be most head time tore. Colonel or passage to ability. 
        </div>
    </section>
</template>




<script>
import BasicDataTute from './BasicDataTute/BasicDataTute.vue'


export default {
    name: 'SectionHome',
    components: {
        BasicDataTute
    },
    data(){
        return{

            show: true,
            // show: false,
            aClass: 'ThirdButton_Color',
            shown: false,
            bacColor: 'green'
        }
    }
}
</script>
<style scoped>
.RandomText{
    border: 1px solid green;
    box-sizing: border-box;
    padding: 5px;
    text-align: justify;
}
.display{
    background-color: fuchsia;
}
.ThirdButton_Color{
    background-color: #fccc72;
    color: green;
}
.yesShow{
    background-color: purple;
    color: white;
}
.noShow{
    background-color: green;
    color: white;
}

</style>