<template>
    <div class="projects">
        <h1>Projects</h1>
        <div class="projects-container">
            <div class="project">
                <img src="../public/images/9.jpg" class="project-image-large">
                <div class="project-data">
                    <div>
                        <img src="../public/projects/gearguard.svg" class="project-image-small">
                    </div>
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

<style lang="css">
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
        padding:10px;
        display: flex;
        flex-direction: column;
        justify-content: space-between;
        position: relative;
        z-index: 2;
        flex-grow: 1;
        gap:4px;
    }
    .project-image-large{
        height:100%;
        width:100%;
        object-fit: cover;
        position:absolute;
        top:0;
    }
    .project-image-small {
        width:32px;
        height:32px;
    }
    .project {
        background-color: rgb(247, 247, 247);
        height: 100px;
        overflow:hidden;
        /* padding:10px; */
        border-radius: 8px;
        display:flex;
        color:white;
        position:relative;
    }
    .project:hover {
        cursor:pointer;
    }
</style>