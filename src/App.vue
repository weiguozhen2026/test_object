<script setup>
import SiteHeader from './components/SiteHeader.vue'
import HeroSection from './components/HeroSection.vue'
import SeasonalMenu from './components/SeasonalMenu.vue'
import StorySection from './components/StorySection.vue'
import VisitSection from './components/VisitSection.vue'
import SiteFooter from './components/SiteFooter.vue'
</script>

<template>
  <SiteHeader />
  <main id="top">
    <HeroSection />
    <div class="ticker" aria-label="餐厅理念"><div class="ticker-inner"><span>顺时而食 <i>✳</i> 山野鲜味 <i>✳</i> 一席一会 <i>✳</i> 顺时而食 <i>✳</i> 山野鲜味 <i>✳</i> 一席一会 <i>✳</i></span></div></div>
    <SeasonalMenu />
    <StorySection />
    <VisitSection />
  </main>
  <SiteFooter />
</template>
