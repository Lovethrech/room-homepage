<script setup>
import { ref } from "vue";
import Nav from "@/components/Nav.vue";

const heroSrc = ref("/desktop-image-hero-1.jpg");
const heroMobileSrc = ref("/mobile-image-hero-1.jpg");
const heroAlt = ref("Image hero one");
const heroTextTitle = ref("Discover innovative ways to decorate");
const heroTextParagraph = ref("We provide unmatched quality, comfort, and style for property owners across the country.Our experts combine form and function in bringing your vision to life. Create a room in your own style with our collection and make your property a reflection of you and what you love.");

const rightClick = () => {
    if (heroSrc.value === "/desktop-image-hero-1.jpg") {
        heroSrc.value = "/desktop-image-hero-2.jpg";
        heroMobileSrc.value = "/mobile-image-hero-2.jpg";
        heroAlt.value = "Image hero two";
        heroTextTitle.value = "We are available all across the globe";
        heroTextParagraph.value = "With stores all over the world, it's easy for you to find furniture for your home or place of business. Locally, we're in most major cities throughout the country. Find the branch nearest you using our store locator. Any questions? Don't hesitate to contact us today";

    }
    else if (heroSrc.value === "/desktop-image-hero-2.jpg") {
        heroSrc.value = "/desktop-image-hero-3.jpg";
        heroMobileSrc.value = "/mobile-image-hero-3.jpg";
        heroAlt.value = "Image hero three";
        heroTextTitle.value = "Manufactured with the best materials";
        heroTextParagraph.value = "Our modern furniture store provide a high level of quality. Our company has invested in advanced technology to ensure that every product is made as perfect and as consistent as possible. With three decades of experience in this industry, we understand what customers want for their home and office.";
    }
    else {
        heroSrc.value = "/desktop-image-hero-1.jpg";
        heroMobileSrc.value = "/mobile-image-hero-1.jpg";
        heroAlt.value = "Image hero one";
        heroTextTitle.value = "Discover innovative ways to decorate";
        heroTextParagraph.value = "We provide unmatched quality, comfort, and style for property owners across the country.Our experts combine form and function in bringing your vision to life. Create a room in your own style with our collection and make your property a reflection of you and what you love.";

    }
}

const leftClick = () => {
    
    if (heroSrc.value === "/desktop-image-hero-1.jpg") {
        heroSrc.value = "/desktop-image-hero-3.jpg";
        heroMobileSrc.value = "/mobile-image-hero-3.jpg";
        heroAlt.value = "Image hero three";
        heroTextTitle.value = "Manufactured with the best materials";
        heroTextParagraph.value = "Our modern furniture store provide a high level of quality. Our company has invested in advanced technology to ensure that every product is made as perfect and as consistent as possible. With three decades of experience in this industry, we understand what customers want for their home and office.";
    }
    else if (heroSrc.value === "/desktop-image-hero-3.jpg") {
        heroSrc.value = "/desktop-image-hero-2.jpg";
        heroMobileSrc.value = "/mobile-image-hero-2.jpg";
        heroAlt.value = "Image hero two";
        heroTextTitle.value = "We are available all across the globe";
        heroTextParagraph.value = "With stores all over the world, it's easy for you to find furniture for your home or place of business. Locally, we're in most major cities throughout the country. Find the branch nearest you using our store locator. Any questions? Don't hesitate to contact us today";

    }

    
    else {
        heroSrc.value = "/desktop-image-hero-1.jpg";
        heroMobileSrc.value = "/mobile-image-hero-1.jpg";
        heroAlt.value = "Image hero one";
        heroTextTitle.value = "Discover innovative ways to decorate";
        heroTextParagraph.value = "We provide unmatched quality, comfort, and style for property owners across the country.Our experts combine form and function in bringing your vision to life. Create a room in your own style with our collection and make your property a reflection of you and what you love.";

    }
}
</script>


<style scoped>
.head-section-main{
    width:100%;
    height:100%;
}
.head-section-main-ctn{
    width:100%;
    height:100%;
}
.head-section-semi-ctn{
    position:fixed;
    z-index:-1;
    display:flex;
    width:100%;
    height:100%;
}
.section-one{
    width:60%;
    height:100%;
}
.nav-mobile{
    display:none;    
}
.section-one-image-desktop img{
    width:100%;
    height:70vh;
}
.section-one-image-mobile{
    display:none;
}
.section-two{
    width:40%;
    height:100%;
}
.head-content-text-main{
    padding:160px 70px;
    width:100%;
    height:100%;
}
.head-content-text-semi-ctn{
    width:100%;
    height:100%;
}
.title{
    font-size: 2vw;
}
.head-title-paragraph{
    line-height:2;
    font-size: 1vw;
}
.shop-content{
    width:100%;
    color:hsl(0, 0%, 0%);
    display:flex;
    text-transform:uppercase;
    font-size: 1.2vw;
    font-weight:400;
    letter-spacing:10px;
}
.shop-content:hover{
    cursor: pointer;
    color:hsla(0, 0%, 0%, 0.336);
}

.visible-content{
    position:fixed;
    width:100%;
}
.nav{
    height:10vh;
}
.nav-btn-semi-ctn{
    width:100%;
    height:60vh;
    display:flex;
    place-items:end;
}
.nav-btn-first-ctn{
    width:60%;
    height:8vh;
}
.nav-btn-main-ctn{
    display:flex;
    width:40%;
    height:8vh;
}
.nav-left-btn, .nav-right-btn, .nav-left-btn-mobile, .nav-right-btn-mobile{
    width:100px;
    background-color: hsl(0, 0%, 0%);
    color:hsl(0, 2%, 61%);
    display:flex;
    place-items:center;
}
.nav-left-btn:hover, .nav-right-btn:hover,.nav-left-btn-mobile:hover, .nav-right-btn-mobile:hover{
    cursor:pointer;
    background-color: hsl(0, 1%, 26%);
    transition: all .5s;
}
.nav-left-btn i, .nav-right-btn i, .nav-left-btn-mobile i, .nav-right-btn-mobile i{
    margin:0 auto;
    font-size:50px;
}
.nav-btn-main-ctn-mobile{
    display:none;
}
.shop-icon i{
    margin: auto 0;
}


@media screen and (max-width:900px) {
    .head-section-semi-ctn{
        position: relative;
        z-index:1;
        display:flex;
        flex-direction: column;
    }
    .section-one{
        width:100%;
        height:70vh;
    }
    .nav-mobile{
        display:flex;
        position:absolute;
        top:0;    
    }
    .section-one-image-desktop img{
        display:none;
        
    }
    .section-one-image-mobile{
        display: flex;
        width:100%;
        height:100%;
    }
    .head-content-text-main{
        padding:30px;
    }
    .section-two{
        width:100%;
        height:100%;
    }
    .title{
        font-size: 30px;
    }
    .head-title-paragraph{
        line-height:2;
        font-size: 16px;
    }
    .shop-content{
        font-size:20px;
    }

    .visible-content-main-ctn{
        width:100%;
        height:41vh;
    }
    .nav {
        position:absolute;
        width:100%;
        height: 10vh;
    }
    .nav-btn-semi-ctn{
        flex-direction:column;
        width:100%;
        height:76%;        
    }
    .nav-btn-first-ctn {
        width: 100%;
        height: 80%;
    }

    .nav-btn-main-ctn {
        display: flex;
        justify-content:end;
        width: 60%;
        height: 6vh;
    }
    .nav-btn-main-ctn-mobile{
        position:absolute;
        top:60.9vh;
        right:0;
        display:flex;
        justify-content:end;
        height:60px;
        width: 100%;
        
    }
    .section-one-image-mobile img{
        width:100%;
    }
}
</style>


<template>
    <div class="head-section-main">
        <div class="head-section-main-ctn">

            <div class="head-section-semi-ctn">
                <div class="section-one">
                    <div class="mobile-interactive-interface">
                        <Nav class="nav-mobile"></Nav>
                        <div class="nav-btn-main-ctn-mobile">
                            <div class="nav-left-btn-mobile" @click="leftClick">
                                <i class='bx bx-chevron-left'></i>
                            </div>
                            <div class="nav-right-btn-mobile" @click="rightClick">
                                <i class='bx bx-chevron-right'></i>
                            </div>
                        </div>
                    </div>

                    <div class="section-one-image-desktop">
                        <img :src="heroSrc" :alt="heroAlt" />
                    </div>
                    <div class="section-one-image-mobile">
                        <img :src="heroMobileSrc" :alt="heroAlt" />
                    </div>
                </div>
                <div class="section-two">
                    <div class="head-content-text-main">
                        <div class="head-content-text-semi-ctn">
                            <h2 class="title">{{ heroTextTitle}}</h2><br />
                            <p class="head-title-paragraph">{{ heroTextParagraph}}</p><br /><br />
                            <div class="shop-content">
                                <p class="shop-name">shop now</p>
                                <div class="shop-icon">
                                    <i class='bx bx-arrow-back bx-rotate-180'></i>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>

            <div class="visible-content">
                <div class="visible-content-main-ctn">
                    <Nav class="nav"></Nav>
                    <div class="nav-btn-semi-ctn">
                        <div class="nav-btn-first-ctn"></div>
                        <div class="nav-btn-main-ctn">
                            <div class="nav-left-btn" @click="leftClick">
                                <i class='bx bx-chevron-left'></i>
                            </div>
                            <div class="nav-right-btn" @click="rightClick">
                                <i class='bx bx-chevron-right'></i>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>

    </div>
</template>
