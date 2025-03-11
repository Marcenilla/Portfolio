<script setup>
import Navbar from '@/components/Navbar.vue';
import SideNav from '@/components/SideNav.vue';
import Index from '@/pages/Index.vue';
</script>

<template >
  <main>
   <div class="hidden md:block" >
     <Navbar />
    </div>
    <div class="block md:hidden">
      <SideNav/>
    </div>
    <section  class="pt-56">
      <Index />
    </section>
  </main>
</template>

<style scoped>

</style>
