<template lang="">
  <header class="text-center border shadow-sm">
    <nav class="uppercase flex justify-between items-center mx-2">
      <ul class="flex">
        <li class="mr-2"><NuxtLink to="/shop">Shop</NuxtLink></li>
        <li><NuxtLink to="/about">About</NuxtLink></li>
      </ul>
      <img src="https://placehold.co/120x60" />
      <ul class="flex">
        <li>
          <input type="text" class="border rounded-sm" placeholder="Search" />
        </li>
        <li class="ml-2"><NuxtLink to="/login">login</NuxtLink></li>
        <li class="ml-2"><NuxtLink to="/cart">cart</NuxtLink></li>
      </ul>
    </nav>
  </header>
</template>
<script>
export default {};
</script>
<style lang=""></style>
