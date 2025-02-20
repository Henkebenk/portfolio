<template>
    <div id="navbar">
        <div id="links">
            <a href="#hero">Hero</a>
            <a href="#game">Technologies</a>
            <a href ="#about">Projects</a>
        </div>
    </div>
</template>

<style scoped>
    #navbar{
        width: 100%;
        margin:0 auto;
        display:flex;
        justify-content: center;
        position: fixed;
        padding:10px;
        top:-100px;
        transition: all 0.5s ease-in-out;
    }
    #navbar a {
        text-decoration: none;
        color:rgb(245, 245, 245);
        font-weight: 500;
    }

    #navbar a:hover {
        color: white;
        cursor:pointer;
    }

    #links {
        background-color: rgba(0, 0, 0, 0.788);
        display:flex;
        justify-content: space-evenly;
        flex-grow: 1;
        max-width: 400px;
        padding:10px;
        border-radius: 24px;
        backdrop-filter: blur(20px);
        box-shadow: rgba(0, 0, 0, 0.05) 0px 1px 2px 0px;
        /* box-shadow: rgba(149, 157, 165, 0.2) 0px 8px 24px; */
    }
</style>

