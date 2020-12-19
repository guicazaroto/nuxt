<template>
  <div>
    <nav>
      <ul class="navbar">
        <li>
          <NuxtLink to="/">Home</NuxtLink>
        </li>
        <li>
          <NuxtLink to="/posts">Posts</NuxtLink>
        </li>
        <li>About</li>
        <li>Blog</li>
      </ul>
    </nav>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.navbar {
  display: flex;
  justify-content: space-between;
  width: 90%;
  max-width: 500px;
  margin: 0 auto;
}
.navbar li {
  list-style-type: none;
}
.navbar li a {
  text-decoration: none;
  color: #b1b108;
}
.navbar li a:hover {
  color: #fff;
}
</style>
