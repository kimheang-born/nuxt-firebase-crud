<template>
  <div class="home-page">
    <section class="intro">
      <h1>Get the latest tech news!</h1>
    </section>
    <PostList />
  </div>
</template>

<script>
import PostList from "@/components/Posts/PostList"

export default {
  name: 'IndexPage',
  components: {
    PostList,
  }
}
</script>

<style lang="scss" scoped></style>
