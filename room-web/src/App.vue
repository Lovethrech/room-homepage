<script setup>
import HeadSection from "@/components/HeadSection.vue";
import FooterContent from "@/components/FooterContent.vue";
</script>

<style scoped>
.app-main{
  width:100%;
  height:100%;
}
.head-section{
  width:100%;
  height:70%;
}
.footer-content{
  width:100%;
  height:30%;
}
</style>


<template>
  <div class="app-main">
    <HeadSection class="head-section"></HeadSection>
    <FooterContent class="footer-content"></FooterContent>
  </div>
</template>