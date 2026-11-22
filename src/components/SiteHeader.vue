<script setup>
import { ref } from 'vue'

const isMenuOpen = ref(false)
const closeMenu = () => { isMenuOpen.value = false }
</script>

<template>
  <header class="wrap">
    <a class="brand" href="#top" aria-label="山隐首页" @click="closeMenu"><span class="brand-mark">山</span><span><span class="brand-name">山隐</span><span class="brand-sub">SHAN YIN · MOUNTAIN CUISINE</span></span></a>
    <button class="menu-toggle" aria-label="打开导航" :aria-expanded="isMenuOpen" @click="isMenuOpen = !isMenuOpen">{{ isMenuOpen ? '×' : '☰' }}</button>
    <nav class="nav" :class="{ open: isMenuOpen }" aria-label="主导航"><a href="#menu" @click="closeMenu">时令菜单</a><a href="#story" @click="closeMenu">关于山隐</a><a href="#visit" @click="closeMenu">寻味地址</a><a class="reserve" href="tel:021-6123-8899" @click="closeMenu">预约席位&nbsp; ↗</a></nav>
  </header>
</template>
