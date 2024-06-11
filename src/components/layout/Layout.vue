<template>
  <Header />
  <OuterHeader />
  <main>
    <slot />
  </main>
  <Footer />
  <BottomNav />
</template>

<script setup>
import Header from "../shared/Header.vue";
import OuterHeader from "../shared/OuterHeader.vue";
import Footer from "../shared/Footer.vue";
import BottomNav from "../shared/BottomNav.vue";
</script>
