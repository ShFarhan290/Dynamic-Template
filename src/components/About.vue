<script setup>
const aboutArea = {
    headingName : "About Me" ,
    titleText : "My name is Start Bootstrap and I help brands grow." ,
    paragraph : "Lorem ipsum dolor sit amet, consectetur adipisicing elit. Fugit dolorum itaque qui unde quisquam consequatur autem. Eveniet quasi nobis aliquid cumque officiis sed rem iure ipsa! Praesentium ratione atque dolorem?" ,

    icons : [
        {iconClass : "bi bi-twitter"},
        {iconClass : "bi bi-linkedin"},
        {iconClass : "bi bi-github"}
    ]
}
</script>

<template>
            <section class="bg-light py-5">
                <div class="container px-5">
                    <div class="row gx-5 justify-content-center">
                        <div class="col-xxl-8">
                            <div class="text-center my-5">
                                <h2 class="display-5 fw-bolder"><span class="text-gradient d-inline">{{ aboutArea.headingName }}</span></h2>
                                <p class="lead fw-light mb-4">{{ aboutArea.titleText }}</p>
                                <p class="text-muted">{{ aboutArea.paragraph }}</p>
                                <div class="d-flex justify-content-center fs-2 gap-4">
                                    <a v-for="icon in aboutArea.icons" :key="icon.iconClass" class="text-gradient" href="#!"><i :class="icon.iconClass"></i></a>
                                    <!-- <a class="text-gradient" href="#!"><i class=""></i></a>
                                    <a class="text-gradient" href="#!"><i class=""></i></a> -->
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </section>
</template>

