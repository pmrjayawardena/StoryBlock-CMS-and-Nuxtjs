<template>
  <section id="posts">
    <PostPreview
      v-for="post in posts"
      :key="post.id"
      :title="post.title"
      :excerpt="post.previewText"
      :thumbnailImage="post.thumbnailUrl"
      :id="post.id"
    />
  </section>
</template>

<script>
import PostPreview from "../components/Blog/PostPreview";
export default {
  components: {
    PostPreview
  },
  data() {
    return {
      posts: [
        {
          id: "1",
          title: "A New Beginning",
          previewText: "This is Awesome",
          thumbnailUrl:
            "https://www.helpguide.org/wp-content/uploads/fast-foods-candy-cookies-pastries-768.jpg"
        },
        {
          id: "2",
          title: "A New Beginning 2",
          previewText: "This is Awesome 2",
          thumbnailUrl:
            "https://www.helpguide.org/wp-content/uploads/fast-foods-candy-cookies-pastries-768.jpg"
        }
      ]
    };
  }
};
</script>

<style scoped>
#posts {
  padding-top: 2rem;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
}

@media (min-width: 35rem) {
  #posts {
    flex-direction: row;
  }
}
</style>
