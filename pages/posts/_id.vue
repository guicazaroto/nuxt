<template>
  <div>
    <article>
      <h1>{{ currentPost.title }}</h1>
      <p>
        {{ currentPost.body }}
      </p>
    </article>
  </div>
</template>

<script>
export default {
  computed: {
    currentPost() {
      return this.$store.state.posts.all.find(
        x => x.id === this.$route.params.id
      );
    }
  }
};
</script>
