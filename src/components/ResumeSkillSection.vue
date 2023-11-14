<script setup>
const skillCard = {
    firstHeading : "Professional Skills" ,
    skills : [
        {name : "SEO/SEM Marketing"},
        {name : "Statistical Analysis"},
        {name : "Web Development"},
        {name : "Network Security"},
        {name : "Adobe Software Suite"},
        {name : "User Interface Design"}
    ],

    secondHeading : "Languages",

    languages : [
        {name : "HTML"},
        {name : "CSS"},
        {name : "JavaScript"},
        {name : "Python"},
        {name : "Ruby"},
        {name : "Node.js"}
    ]
}
</script>

<template>
    <div class="pb-5"></div>
    <!-- Skills Section-->
    <section>
        <!-- Skillset Card-->
        <div class="card shadow border-0 rounded-4 mb-5">
            <div class="card-body p-5">
                <!-- Professional skills list-->
                <div class="mb-5">
                    <div class="d-flex align-items-center mb-4">
                        <div class="feature bg-primary bg-gradient-primary-to-secondary text-white rounded-3 me-3"><i class="bi bi-tools"></i></div>
                        <h3 class="fw-bolder mb-0"><span class="text-gradient d-inline">{{ skillCard.firstHeading }}</span></h3>
                    </div>
                    <div class="row row-cols-1 row-cols-md-3 mb-4 grid gap-0 row-gap-3">

                        <div  v-for="skill in skillCard.skills" :key="skill.name" class="col mb-4 mb-md-0 p-2 g-col-6"><div class="d-flex align-items-center bg-light rounded-4 p-3 h-100">{{ skill.name }}</div></div>
                        
                    </div>
                </div>
                <!-- Languages list-->
                <div class="mb-0">
                    <div class="d-flex align-items-center mb-4">
                        <div class="feature bg-primary bg-gradient-primary-to-secondary text-white rounded-3 me-3"><i class="bi bi-code-slash"></i></div>
                        <h3 class="fw-bolder mb-0"><span class="text-gradient d-inline">{{ skillCard.secondHeading }}</span></h3>
                    </div>
                    <div class="row row-cols-1 row-cols-md-3 mb-4 grid gap-0 row-gap-3">

                        <div v-for="language in skillCard.languages" :key="language.name" class="p-2 g-col-6 col mb-4 mb-md-0"><div class="d-flex align-items-center bg-light rounded-4 p-3 h-100">{{ language.name }}</div></div>
                        
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

