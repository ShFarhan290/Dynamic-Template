<script setup>
const educationCard = {
    heading : "Education" ,
    cardOne : {
        year : "2015 - 2017",
        collegeName : "Barnett College" ,
        location : "Fairfield, NY" ,
        class : "Master's" ,
        subject : "Web Development" , 
        titleText : "Lorem ipsum dolor sit amet consectetur adipisicing elit. Delectus laudantium, voluptatem quis repellendus eaque sit animi illo ipsam amet officiis corporis sed aliquam non voluptate corrupti excepturi maxime porro fuga."
    },
    cardTwo : {
        year : "2011 - 2015",
        collegeName : "ULA" ,
        location : "Los Angeles, CA" ,
        class : "Undergraduate" ,
        subject : "Computer Science" , 
        titleText : "Lorem ipsum dolor sit amet consectetur adipisicing elit. Delectus laudantium, voluptatem quis repellendus eaque sit animi illo ipsam amet officiis corporis sed aliquam non voluptate corrupti excepturi maxime porro fuga."
    },

};
</script>

<template>
    <section>
        <h2 class="text-secondary fw-bolder mb-4">{{ educationCard.heading }}</h2>
        <!-- Education Card 1-->
        <div class="card shadow border-0 rounded-4 mb-5">
            <div class="card-body p-5">
                <div class="row align-items-center gx-5">
                    <div class="col text-center text-lg-start mb-4 mb-lg-0">
                        <div class="bg-light p-4 rounded-4">
                            <div class="text-secondary fw-bolder mb-2">{{ educationCard.cardOne.year }}</div>
                            <div class="mb-2">
                                <div class="small fw-bolder">{{ educationCard.cardOne.collegeName }}</div>
                                <div class="small text-muted">{{ educationCard.cardOne.location }}</div>
                            </div>
                            <div class="fst-italic">
                                <div class="small text-muted">{{ educationCard.cardOne.class }}</div>
                                <div class="small text-muted">{{ educationCard.cardOne.subject }}</div>
                            </div>
                        </div>
                    </div>
                    <div class="col-lg-8"><div>{{ educationCard.cardOne.titleText }}</div></div>
                </div>
            </div>
        </div>
        <!-- Education Card 2-->
        <div class="card shadow border-0 rounded-4 mb-5">
            <div class="card-body p-5">
                <div class="row align-items-center gx-5">
                    <div class="col text-center text-lg-start mb-4 mb-lg-0">
                        <div class="bg-light p-4 rounded-4">
                            <div class="text-secondary fw-bolder mb-2">{{ educationCard.cardTwo.year }}</div>
                            <div class="mb-2">
                                <div class="small fw-bolder">{{ educationCard.cardTwo.collegeName }}</div>
                                <div class="small text-muted">{{ educationCard.cardTwo.location }}</div>
                            </div>
                            <div class="fst-italic">
                                <div class="small text-muted">{{ educationCard.cardTwo.class }}</div>
                                <div class="small text-muted">{{ educationCard.cardTwo.subject }}</div>
                            </div>
                        </div>
                    </div>
                    <div class="col-lg-8"><div>{{ educationCard.cardTwo.titleText }}</div></div>
                </div>
            </div>
        </div>
    </section>
</template>
