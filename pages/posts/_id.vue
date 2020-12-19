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
  data() {
    return {
      articles: [
        {
          id: "first",
          title: "First Post",
          body:
            "Lorem ipsum dolor sit amet consectetur adipisicing elit. Sint eligend voluptatum iusto quaerat suscipit corporis distinctio omnis dicta, eiusquasi eaque? Deserunt veniam, corporis doloribus in suscipit fugiat velit odit."
        },
        {
          id: "second",
          title: "Second Post",
          body:
            "Lorem ipsum dolor sit amet consectetur adipisicing elit. Sint eligend voluptatum iusto quaerat suscipit corporis distinctio omnis dicta, eiusquasi eaque? Deserunt veniam, corporis doloribus in suscipit fugiat velit odit."
        },
        {
          id: "third",
          title: "Third Post",
          body:
            "Lorem ipsum dolor sit amet consectetur adipisicing elit. Sint eligend voluptatum iusto quaerat suscipit corporis distinctio omnis dicta, eiusquasi eaque? Deserunt veniam, corporis doloribus in suscipit fugiat velit odit."
        }
      ]
    };
  },
  computed: {
    currentPost() {
      return this.articles.find(x => x.id === this.$route.params.id);
    }
  }
};
</script>
