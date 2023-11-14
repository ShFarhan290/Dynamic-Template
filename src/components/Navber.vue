<script setup>
const navbarData = {
    websiteName : {name : "Doofaz IT Limited" , url : "index.html"},
    menuItems : [
        {name : "Home" , url : "./"},
        {name : "Resume" , url : "./resume"},
        {name : "Project" , url : "./project"},
        {name : "Contact" , url : "./contact"}
    ],
};
</script>

<template>
    <nav class="navbar navbar-expand-lg navbar-light bg-white py-3">
        <div class="container px-5">
            <a class="navbar-brand" :href="navbarData.websiteName.url"><span class="fw-bolder text-primary">{{ navbarData.websiteName.name }}</span></a>
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation"><span class="navbar-toggler-icon"></span></button>
            <div class="collapse navbar-collapse" id="navbarSupportedContent">
                <ul class="navbar-nav ms-auto mb-2 mb-lg-0 small fw-bolder">

                    <li v-for="menu in navbarData.menuItems" :key="menu.name" class="nav-item">
                        <RouterLink :to="menu.url" class="nav-link">{{ menu.name }}</RouterLink>
                    </li>
                    
                </ul>
            </div>
        </div>
    </nav>
</template>

<style scoped>
</style>