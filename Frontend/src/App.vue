<script setup>
import { useRoute } from 'vue-router';
import Navbar from './components/Navbar.vue';
import Hero from './components/Hero.vue';
import Categories from './components/Categories.vue';
import PopularProducts from './components/PopularProducts.vue';
import Footer from './components/Footer.vue';

// เข้าถึง route ปัจจุบัน
// const route = useRoute();
</script>

<!-- แสดง Navbar และ Hero เฉพาะเมื่อไม่ใช่หน้า login -->
<template>

    <Navbar />

    <Hero />

    <Categories />

    <PopularProducts />
    <router-view></router-view>

    <!-- แสดง Footer เฉพาะเมื่อไม่ใช่หน้า login -->
    <Footer/>
</template>

<style scoped>
</style>
