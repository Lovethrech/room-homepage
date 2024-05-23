<script setup>
import {ref} from "vue";

const menuOpen = ref("<i class='bx bx-menu'></i>");
const mainNavBg = ref("transparent");
const iconColor = ref("white");
const logoDisplay = ref("flex");
const mobileNavDisplay = ref("none");

const menuBarClick=()=>{
    if (menuOpen.value === "<i class='bx bx-menu'></i>") {
        menuOpen.value = "<i class='bx bx-x'></i>";
        mainNavBg.value = "white";
        iconColor.value = "black";
        logoDisplay.value = "none";
        mobileNavDisplay.value = "flex";
    }
    else {
        menuOpen.value = "<i class='bx bx-menu'></i>";
        mainNavBg.value = "transparent";
        iconColor.value = "white";
        logoDisplay.value = "flex";
        mobileNavDisplay.value = "none";
    }
}    
</script>

<style scoped>
.nav-main-ctn{
    padding:4vh 3vw;
}
.nav-main{
    display:flex;
    gap:70px;
}
.menu-icon-ctn{
    display:flex;
    place-items: center;
    width:40px;
    height:100%;
    font-size:30px;
    margin:auto 0;
}
.menu-icon-ctn {
    display:none;
}
.logo-image-ctn:hover{
    cursor:pointer;
}
.nav-list-ctn{
    list-style:none;
    display:flex;
    place-items:center;
    gap:40px;
}
.nav-list{
    color:hsl(0, 0%, 100%);
    text-transform:lowercase;
}
.nav-list:hover{
    cursor:pointer;
    text-decoration:underline;
    text-decoration-line:20px;
}
.logo-image-ctn{
    display: flex;
    place-items: center;
}
.nav-list-ctn-mobile{
    list-style: none;
    justify-content: space-evenly;
    gap:20px;
    width:80%;
}
.mobile-nav-list{
    font-weight:600;
    margin:auto 0;
    text-transform: lowercase;
}
.mobile-nav-list:hover {
    cursor:pointer;
}

@media screen and (max-width:900px){
    .nav{
        justify-content: space-between;
        
    }
    .nav-main {
        gap: 120px;
        width: 100vw;
    }
    .nav-list-ctn{
        display:none;
    }
    .logo-image-ctn{
        width:80%;
        padding-right:32vw;
    }
    .logo-image-ctn img{
        margin: 0 auto;
    }
    .menu-icon-ctn{
        display: flex;
        width:30px;
        margin:0;
        padding:0;
    }
    .menu-icon-ctn:hover{
        cursor:pointer;
    }
}
</style>


<template>
    <div class="nav-main-ctn" :style="{backgroundColor:mainNavBg}">
        <div class="nav-main">
            <div 
                v-html="menuOpen" 
                class="menu-icon-ctn" 
                @click="menuBarClick"
                :style="{ color: iconColor }"
            >
            </div>
            <div class="logo-image-ctn" :style="{ display: logoDisplay }">
                <img src="/public/logo.svg" alt="" />
            </div>
            <ul class="nav-list-ctn">
                <li class="nav-list">Home</li>
                <li class="nav-list">Shop</li>
                <li class="nav-list">About</li>
                <li class="nav-list">Contact</li>
            </ul>

            <ul class="nav-list-ctn-mobile" :style="{ display: mobileNavDisplay }">
                <li class="mobile-nav-list">Home</li>
                <li class="mobile-nav-list">Shop</li>
                <li class="mobile-nav-list">About</li>
                <li class="mobile-nav-list">Contact</li>
            </ul>

        </div>
    </div>
</template>
