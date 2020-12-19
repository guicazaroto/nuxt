<template>
  <div>
    <h1>Posts here</h1>
    <p>
      <NuxtLink to="/posts/first">First</NuxtLink>
    </p>
    <p>
      <NuxtLink to="/posts/second">Second</NuxtLink>
    </p>
  </div>
</template>

<style scoped>
p a {
  text-decoration: none;
  color: #b1b108;
}
p a:hover {
  color: #fff;
}
</style>
