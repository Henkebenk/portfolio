<template>
    <div class="techniques">
        <h1>Current technologies</h1>
        <div class="techniques-container">
            <div class="technique">
                <div class="icon" style="background-color: #41B8833A;">
                    <img src="../public/icons/vue.svg">
                </div>
                <label>Vue</label>
            </div>
            <div class="technique">
                <div class="icon" style="background-color: #44A8B32E;">
                    <img src="../public/icons/tailwind.svg">
                </div>
                <label>Tailwind</label>
            </div>
            <div class="technique">
                <div class="icon" style="background-color: #6CCEF24B;">
                    <img src="../public/icons/flutter.svg">
                </div>
                <label>Flutter</label>
            </div>
            <div class="technique">
                <div class="icon" style="background-color: #8CC84B2B;">
                    <img src="../public/icons/node.svg">
                </div>
                <label>Node</label>
            </div>
            <div class="technique">
                <div class="icon" style="background-color: #0000001E;">
                    <img src="../public/icons/next.svg">
                </div>
                <label>NextJS</label>
            </div>
            <div class="technique">
                <div class="icon" style="background-color: #904BC825;">
                    <img src="../public/icons/figma.svg">
                </div>
                <label>Figma</label>
            </div>
            <div class="technique">
                <div class="icon" style="background-color: #EE5D283B;">
                    <img src="../public/icons/html.svg">
                </div>
                <label>HTML</label>
            </div>
            <div class="technique">
                <div class="icon" style="background-color: #33AADD30;">
                    <img src="../public/icons/css.svg">
                </div>
                <label>CSS</label>
            </div>
            <div class="technique">
                <div class="icon" style="background-color: #F7DE1E57;">
                    <img src="../public/icons/javascript.svg">
                </div>
                <label>Javascript</label>
            </div>
        </div>
    </div>
</template>

<style lang="css">
    .techniques {
        width: 100%;
        display:flex;
        flex-direction: column;
        gap:8px;
    }
    .techniques-container {
        display:grid;
        grid-template-columns: repeat(4, 1fr);
        gap: 10px;
    }
    .technique{
        background-color: rgb(247, 247, 247);
        height: 40px;
        padding:10px;
        border-radius: 8px;
        display:flex;
        flex-direction: row;
        justify-content: left;
        align-items: center;
        gap:8px;
    }
    .icon {
        width:36px;
        height:36px;
        display: flex;
        justify-content: center;
        align-items: center;
        border-radius: 8px;
    }
    .technique img {
        width:24px;
        height:24px;
    }
</style>