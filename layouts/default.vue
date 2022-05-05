<template>
  <div>
    <div class="nav">
      <NuxtLink class="link" :to="{ name: 'index' }">Home</NuxtLink>
      <NuxtLink class="link" :to="{ name: 'about' }">About</NuxtLink>
      <NuxtLink class="link" :to="{ name: 'contact' }">Contact</NuxtLink>
    </div>
    <slot />
  </div>
</template>
<style scoped>
.link {
  background-color: blueviolet;
  color: white;
  padding: 6px;
  border-radius: 24px;
  text-decoration: none;
}
.nav {
  gap: 9px;
  display: flex;
}
</style>