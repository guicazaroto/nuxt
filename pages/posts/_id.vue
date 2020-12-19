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
  head() {
    return {
      title: this.currentPost.title,
      meta: [
        { name: "twitter:title", content: this.currentPost.title },
        { name: "twitter:description", content: this.currentPost.body },
        { name: "twitter:image", content: "https://img.com.br/img.png" },
        { name: "twitter:card", content: "summary_large_image" }
      ]
    };
  },
  computed: {
    currentPost() {
      return this.$store.state.posts.all.find(
        x => x.id === this.$route.params.id
      );
    }
  }
};
</script>
