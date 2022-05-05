<template>
  <div class="content">
    <div class="bar">
      <NuxtLink class="brand" :to="{ name: 'index' }"><img src="/y.svg" class="logo"/></NuxtLink>
      <div class="nav">
        <NuxtLink class="link" :to="{ name: 'index' }">Home</NuxtLink>
        <NuxtLink class="link" :to="{ name: 'about' }">About</NuxtLink>
        <NuxtLink class="link" :to="{ name: 'contact' }">Contact</NuxtLink>
      </div>
    </div>
    <slot />
  </div>
</template>
<style scoped>
.link {
  background-color: rgb(43, 95, 226);
  color: white;
  padding: 6px 32px;
  border-radius: 4px;
  text-decoration: none;
}
.nav {
  gap: 9px;
  display: flex;
}
.bar {
  display: flex;
  justify-content: space-between;
  background-color: lightpink;
  align-items: center;
}
.content {
  font-family: Arial, Helvetica, sans-serif;
}
.brand {
  display: flex;
  align-items: center;
}
.logo {
  width: 128px;
}
</style>
