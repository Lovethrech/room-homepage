<style scoped>
.nav-main-ctn{
    background-color: transparent;
    padding:4vh 3vw;
}
.nav-main{
    display:flex;
    gap:70px;
}
.nav-list-ctn{
    list-style:none;
    display:flex;
    gap:40px;
}
.nav-list{
    color:hsl(0, 0%, 100%);
    text-transform:lowercase;
}
</style>


<template>
    <div class="nav-main-ctn">
        <div class="nav-main">
            <div class="logo-image-ctn">
                <img src="/public/logo.svg" alt=""/>
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