<script setup>
import Navbar from '@/components/Navbar.vue';
import SideNav from '@/components/SideNav.vue';
import TheFooter from '@/components/TheFooter.vue';
import LoadingAnimation from '@/components/LoadingAnimation.vue';
import Index from '@/pages/Index.vue';
</script>

<template>
  <main>
    <div class="hidden md:block">
      <Navbar />
    </div>
    <div class="block md:hidden">
      <SideNav />
    </div>

    <div>
      <LoadingAnimation />
    </div>
    <section class="pt-40 ">
      <Index />
    </section>
  </main>
  <TheFooter />
</template>

<style scoped></style>
