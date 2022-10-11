<template>
  <div class="home-page">
    <section class="intro">
      <h1>Get the latest tech news!</h1>
    </section>
    <section class="featured-posts">
      <PostPreview 
        id="1"
        thumbnail="https://cdn.sabay.com/cdn/media.sabay.com/media/sabay-news/Sport-News/International-Sports/soccer/Soccer54/Soccer144/Soccer212/634386e3ea970_1665369780_large.jpg"
        title="Hello"
        previewText="This is my text."
      />
      <PostPreview 
        id="2"
        thumbnail="https://cdn.sabay.com/cdn/media.sabay.com/media/sabay-news/Sport-News/International-Sports/soccer/Soccer54/Soccer144/Soccer212/634386e3ea970_1665369780_large.jpg"
        title="Hello"
        previewText="This is my text."
      />
    </section>
  </div>
</template>

<script>
import PostPreview from "@/components/Posts/PostPreview"

export default {
  name: 'IndexPage',
  components: {
    PostPreview,
  }
}
</script>

<style lang="scss" scoped></style>
