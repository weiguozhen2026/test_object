<script setup>
const dishes = [
  { name: '春笋 · 青梅 · 山胡椒', ingredients: '当日鲜笋 / 青梅汁 / 山野香草', price: '¥ 88', image: 'https://images.unsplash.com/photo-1547592180-85f173990554?auto=format&fit=crop&w=900&q=85', alt: '时令山野蔬菜与香草' },
  { name: '炭烤 · 谷饲 · 栗木香', ingredients: '谷饲牛小排 / 栗木炭火 / 野菌汁', price: '¥ 188', image: 'https://images.unsplash.com/photo-1544025162-d76694265947?auto=format&fit=crop&w=900&q=85', alt: '炭火慢烤的时令肉料理' },
  { name: '野莓 · 米酿 · 桂花', ingredients: '山野莓果 / 手作米酿 / 桂花蜜', price: '¥ 58', image: 'https://images.unsplash.com/photo-1488477181946-6428a0291777?auto=format&fit=crop&w=900&q=85', alt: '以时令果实制作的餐后甜点' },
]
</script>

<template>
  <section id="menu" class="wrap"><div class="section-head"><h2 class="section-title"><small>SEASONAL MENU · 2026</small>这一季的暖心滋味</h2><p class="section-desc">把山野里刚刚好的新鲜带回餐桌，愿每一道菜，都让你感到被季节温柔款待。</p></div><div class="dishes"><article v-for="dish in dishes" :key="dish.name" class="dish"><div class="dish-image"><img :src="dish.image" :alt="dish.alt" /></div><div class="dish-caption"><div><h3>{{ dish.name }}</h3><p>{{ dish.ingredients }}</p></div><span class="price">{{ dish.price }}</span></div></article></div></section>
</template>
