<template>
    <div class="Home_Header">
        <header>This is Header</header>
        <nav>This is Navbar</nav>
        <aside class="Show_and_HideAside">This is Aside Section</aside>
            <SectionHome/>
        <footer>This is footer</footer>
    </div>
</template>

<script>


import SectionHome from './SectionHome'

export default {
    name: 'MainHome',
    components:{
        SectionHome
    }
}
</script>

<style>
header{
    height: 40px;
    width: 100%;
    position: fixed;
    background: #fffffff5;
    z-index: 800;
    transition: 0.3s;
}
nav{
    height: 40px;
    width: 100%;
    background: rgba(240, 97, 44, 0.604);
    padding-top: 40px;
    position: fixed;
    transition: 0.3s;
}
aside{
    height: 100vh;
    width: 100%;
    background: rgba(172, 255, 47, 0.631);
    position: fixed;
    z-index: 1000;
    transition: 0.3s;
}
section{
    padding-top: 80px;
    padding-bottom: 40px;
    
    /* margin-bottom: 40px; */
    width: 100%;
    min-height: 100vh;
    /* border: 5px solid orange; */
    box-sizing: border-box;
    transition: 0.3s;  
}
footer{
    height: 40px;
    width: 100%;
    background: #fffffff5;
    position: fixed;
    bottom: 0;
    transition: 0.3s;
}

@media only screen and (min-width: 620px){
    header{
        width: 70%;
    }
    nav{
        width: 70%;
    }
    aside{
        width: 30%;
        margin-left: 70%;
    }
    section{
        width: 70%;
    }
    footer{
        width: 70%;
    }
}

@media only screen and (max-width: 620px){

    .Show_and_HideAside{
        display: none;
    }
}

@media only screen and (min-width: 750px){
    header{
        width: 75%;
    }
    nav{
        width: 75%;
    }
    aside{
        width: 25%;
        margin-left: 75%;
    }
    section{
        width: 75%;
    }
    footer{
        width: 75%;
    }
}

@media only screen and (min-width: 1200px){
    header{
        width: 84%;
    }
    nav{
        width: 84%;
    }
    aside{
        width: 16%;
        margin-left: 84%;
    }
    section{
        width: 84%;
    }
    footer{
        width: 84%;
    }
    
}

</style>