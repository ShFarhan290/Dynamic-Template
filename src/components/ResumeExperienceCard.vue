<script setup>
const experienceCard = {
    heading : "Experience" ,
    cardOne : {
        year : "2019 - Present",
        occupation : "Web Developer" ,
        companyName : "Stark Industries" ,
        location : "Los Angeles, CA" , 
        titleText : "Lorem ipsum dolor sit amet consectetur adipisicing elit. Delectus laudantium, voluptatem quis repellendus eaque sit animi illo ipsam amet officiis corporis sed aliquam non voluptate corrupti excepturi maxime porro fuga."
    },
    cardTwo : {
        year : "2017 - 2019",
        occupation : "SEM Specialist" ,
        companyName : "Wayne Enterprises" ,
        location : "Gotham City, NY" , 
        titleText : "Lorem ipsum dolor sit amet consectetur adipisicing elit. Delectus laudantium, voluptatem quis repellendus eaque sit animi illo ipsam amet officiis corporis sed aliquam non voluptate corrupti excepturi maxime porro fuga."
    },

};
</script>

<template>
    <section>
        <div class="d-flex align-items-center justify-content-between mb-4">
            <h2 class="text-primary fw-bolder mb-0"></h2>
            <!-- Download resume button-->
            <!-- Note: Set the link href target to a PDF file within your project-->
            <a class="btn btn-primary px-4 py-3" href="#!">
                <div class="d-inline-block bi bi-download me-2"></div>
                Download Resume
            </a>
        </div>
        <!-- Experience Card 1-->
        <div class="card shadow border-0 rounded-4 mb-5">
            <div class="card-body p-5">
                <div class="row align-items-center gx-5">
                    <div class="col text-center text-lg-start mb-4 mb-lg-0">
                        <div class="bg-light p-4 rounded-4">
                            <div class="text-primary fw-bolder mb-2">{{ experienceCard.cardOne.year }}</div>
                            <div class="small fw-bolder">{{ experienceCard.cardOne.occupation }}</div>
                            <div class="small text-muted">{{ experienceCard.cardOne.companyName }}</div>
                            <div class="small text-muted">{{ experienceCard.cardOne.location }}</div>
                        </div>
                    </div>
                    <div class="col-lg-8"><div>{{ experienceCard.cardOne.titleText }}</div></div>
                </div>
            </div>
        </div>
        <!-- Experience Card 2-->
        <div class="card shadow border-0 rounded-4 mb-5">
            <div class="card-body p-5">
                <div class="row align-items-center gx-5">
                    <div class="col text-center text-lg-start mb-4 mb-lg-0">
                        <div class="bg-light p-4 rounded-4">
                            <div class="text-primary fw-bolder mb-2">{{ experienceCard.cardTwo.year }}</div>
                            <div class="small fw-bolder">{{ experienceCard.cardTwo.occupation }}</div>
                            <div class="small text-muted">{{ experienceCard.cardTwo.companyName }}</div>
                            <div class="small text-muted">{{ experienceCard.cardTwo.location }}</div>
                        </div>
                    </div>
                    <div class="col-lg-8"><div>{{ experienceCard.cardTwo.titleText }}</div></div>
                </div>
            </div>
        </div>
    </section>
</template>

