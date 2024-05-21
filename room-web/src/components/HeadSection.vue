<script setup>
import Nav from "@/components/Nav.vue";
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
.section-one img{
    width:100%;
    height:70vh;
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
    font-size:40px;
}
.head-title-paragraph{
    line-height:2;
    font-size:14px;
}
.shop-content{
    display:flex;
    text-transform:uppercase;
    font-size:22px;
    font-weight:400;
    letter-spacing:10px;
}

.visible-content{
    position:fixed;
    width:100%;
}
.visible-content-main-ctn{

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
.nav-left-btn, .nav-right-btn{
    width:100px;
    background-color: hsl(0, 0%, 0%);
    color:hsl(0, 0%, 100%);
    display:flex;
    place-items:center;

}
.nav-left-btn i, .nav-right-btn i{
    margin:0 auto;
    font-size:50px;
}

.nav-right-btn{

}
</style>


<template>
    <div class="head-section-main">
        <div class="head-section-main-ctn">

            <div class="head-section-semi-ctn">
                <div class="section-one">
                    <div class="section-one-image">
                        <img src="/public/desktop-image-hero-1.jpg" alt=""/>
                    </div>
                </div>
                <div class="section-two">
                    <div class="head-content-text-main">
                        <div class="head-content-text-semi-ctn">
                            <h2 class="title">Discover innovative ways to decorate</h2><br/>
                            <p class="head-title-paragraph">
                                We provide unmatched quality, comfort, and style for property owners across the country.
                                Our experts combine form and function in bringing your vision to life. Create a room in your
                                own style with our collection and make your property a reflection of you and what you love.
                            </p><br/><br/>
                            <div class="shop-content">
                                <p class="shop-name">shop now</p>
                                <div class="shop-icon">
                                    <img src="/public/icon-arrow.svg" alt="arrow-forward"/>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div> 

            <div class="visible-content">
                <div class="visible-content-main-ctn">
                    <Nav></Nav>
                    <div class="nav-btn-semi-ctn">
                        <div class="nav-btn-first-ctn"></div>
                        <div class="nav-btn-main-ctn">
                            <div class="nav-left-btn">
                                <i class='bx bx-chevron-left'></i>
                            </div>
                            <div class="nav-right-btn">
                                <i class='bx bx-chevron-right' ></i>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        
    </div>
</template>