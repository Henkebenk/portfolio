<template>
    <div class="projects">
        <h1>Projects</h1>
        <div class="projects-container">
            <div class="project">
                <div class="project-data">
                    <img src="../public/images/9.jpg">
                    <label>Gearguard</label>
                </div>
            </div>
            <div class="project">
                <div class="project-data">
                    <label>Bytegrave</label>
                    <!-- <div class="chips">
                        <label class="chip">C++</label>
                        <label class="chip">sfml</label>
                        <label class="chip">Doxygen</label>
                    </div> -->
                </div>
            </div>
            <div class="project">
                <label>Hello</label>
            </div>
            <div class="project">
                <label>Hello</label>
            </div>
            <div class="project">
                <label>Hello</label>
            </div>
            <div class="project">
                <label>Hello</label>
            </div>
            <div class="project">
                <label>Hello</label>
            </div>
            <div class="project">
                <label>Hello</label>
            </div>
        </div>
    </div>
</template>

<style lang="css" scoped>
    .chips {
        display:flex;
        flex-direction: row;
        gap:4px;
    }
    .chip {
        color: rgb(92 135 246);
        background-color: rgb(213, 213, 213);
        background-color: #7DA4FF39;
        padding:2px 6px 2px 6px;
        border-radius: 4px;
        font-size: 12px;
    }
    .projects {
        width: 100%;
        display:flex;
        flex-direction: column;
        gap:8px;
        }
    .projects-container {
        display:grid;
        grid-template-columns: repeat(3, 1fr);
        gap: 10px;
    }
    .project-data {
        height:100px;
        position:absolute;
        bottom:8px;
        left:8px;
        /* font-weight: bold; */
        display:flex;
        flex-direction:row;
        /* justify-content: end; */
        gap:4px;
    }
    .project-data img{
        height:100%;
        width:100px;
        object-fit: cover;
        border-radius: 8px;
    }
    .project {
        background-color: rgb(247, 247, 247);
        height: 100px;
        padding:10px;
        border-radius: 8px;
        display:block;
        position:relative;
    }
    .project:hover {
        cursor:pointer;
    }
</style>