<script setup>
    import { Map } from 'lucide-vue-next';
    import { Github } from 'lucide-vue-next';
    import { Mail } from 'lucide-vue-next';
    import { Gitlab } from 'lucide-vue-next';

</script>

<template>
    <div class="hero">
        <label class="hero-header">Hello, I'm <label style="font-weight: bold;">Henrik</label></label>
        <label>Programming student at LiU</label>
        <div class="about">
            <div class="temp">
                <Map stroke-width="1.5"/>
                <!-- <img src="../public/icons/map-pin.svg"> -->
                <p>Linköping, Sweden</p>
            </div>
            <div class="socials">
                <a>
                    <Github stroke-width="1.5" size="20"/>
                </a>
                <a>
                    <Mail stroke-width="1.5" size="20"/>
                </a>
                <a>
                    <Gitlab stroke-width="1.5" size="20"/>
                </a>
            </div>
        </div>
    </div>
</template>

<style>
.socials {
    display: flex;
    gap:4px;
}
.socials a {
    color: white;
    background-color: #464646FF;
    width:28px;
    height:28px;
    display: flex;
    justify-content: center;
    align-items: center;
    border-radius: 8px;
}
.socials a:hover {
    cursor: pointer;
    background-color: #2B2B2BFF;
}
.about {
    display: flex;
    flex-direction: column;
    gap: 8px;
    justify-content: center;
    align-items: center;
}
.temp {
    display: flex;
    justify-content: center;
    gap: 8px;
    align-items: center;
}
.temp p {
    margin: 0;
}
.hero {
    display:flex;
    flex-direction: column;
    justify-content: center;
    max-width:100vw;
    height:100vh;
    text-align: center;
}
.hero-header {
    font-size: 48px;
}
h3 {
    margin: 0;
}
</style>