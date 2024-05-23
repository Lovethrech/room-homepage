<style scoped>
.footer-section-main{
    width:100%;
    height:100%;
}
.footer-section-main-ctn{
    width:100%;
    height:100%;
}
.footer-section-semi-ctn{
    position:fixed;
    z-index:-1;
    display:flex;
    width:100%;
    height:100%;
}
.section-image-main{
    width:30%;
    height:100%;
}
.section-image-main img{
    width:100%;
    height:30vh;
}
.section-two{
    width:40%;
    height:100%;
}
.footer-content-text-main{
    padding: 30px 50px;
    width:100%;
    height:100%;
}
.footer-content-text-semi-ctn{
    width:100%;
    height:100%;
}
.title{
    font-size:1.3vw;
    text-align:center;
    text-transform:uppercase;
    letter-spacing:10px;
}
.footer-title-paragraph{
    line-height:2;
    font-size:1vw;
}

@media screen and (max-width:900px){
    .footer-section-main{
        display: ;
    }
    .footer-section-semi-ctn{
        position:relative;
        z-index:1;
        flex-direction: column;
    }

    .section-image-main, .section-two{
        width:100%;
    }
    .section-image-main img{
        width:100%;
        height:100%;
    }
    .title{
        font-size:18px;
        text-align:left;
        line-height:2;
    }
    .footer-title-paragraph{
        font-size:16px;
    }
    .footer-content-text-main{
        padding:30px;
    }
}
</style>



<template>
    <div class="footer-section-main">
        <div class="footer-section-main-ctn">

            <div class="footer-section-semi-ctn">
                <div class="section-image-main">
                    <div class="section-image-main-image">
                        <img src="/public/image-about-dark.jpg" alt=""/>
                    </div>
                </div>
                <div class="section-two">
                    <div class="footer-content-text-main">
                        <div class="footer-content-text-semi-ctn">

                            <h2 class="title">About our furniture</h2><br/>
                            <p class="footer-title-paragraph">
                                Our multifunctional collection blends design and function to suit your individual taste.
                                Make each room unique, or pick a cohesive theme that best express your interests and what inspires you.
                                Find the furniture pieces you need, from traditional to contemporary styles or anything in between.
                                Product specialists are available to help you create your dream space.
                            </p>
                        </div>
                    </div>
                </div>

                <div class="section-image-main">
                    <div class="section-image-main-image">
                        <img src="/public/image-about-light.jpg" alt=""/>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>