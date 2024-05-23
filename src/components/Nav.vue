<script setup>
import { defineProps } from "vue";

const { menuBarClick } = defineProps(['menuBarClick']);
</script>

<style scoped>
.nav-main-ctn{
    background-color: transparent;
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
    color:hsl(0, 0%, 100%);
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


@media screen and (max-width:900px){
    .nav{
        justify-content: space-around;
        gap:2px;
    }
    .nav-list-ctn{
        display:none;
    }
    .logo-image-ctn{
        position:fixed;
        top:5.2vh;
        left:25vw;
        right:25vw; 
        width:80%;
        padding-left:20vw;
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
    <div class="nav-main-ctn">
        <div class="nav-main">
            <div class="menu-icon-ctn" @click="menuBarClick">
                <i class='bx bx-menu'></i>
            </div>
            <div class="logo-image-ctn">
                <img src="/public/logo.svg" alt="" />
            </div>
            <ul class="nav-list-ctn">
                <li class="nav-list">Home</li>
                <li class="nav-list">Shop</li>
                <li class="nav-list">About</li>
                <li class="nav-list">Contact</li>
            </ul>
        </div>
    </div>
</template>