<template>
  <div>
    <nav>
      <ul class="navbar">
        <li>Home</li>
        <li>Posts</li>
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
</style>
