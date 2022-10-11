<template>
    <div class="posts-page">
        <PostList />
    </div>
</template>

<script>
import PostList from "@/components/Posts/PostList"

export default {
    components: {
      PostList,
    }
}
</script>

<style lang="scss">
.posts-page {
    display: flex;
    justify-content: center;
    text-align: center;
}
.post-list {
  display: flex;
  padding: 20px;
  box-sizing: border-box;
  flex-wrap: wrap;
  align-content: center;
  justify-content: center;

  .post-preview {
    border: 1px solid #ccc;
    box-shadow: 0 2px 2px #ccc;
    background-color: white;
    width: 90%;
  }
  .post-thumbnail {
    width: 100%;
    height: 200px;
    background-position: center;
    background-size: cover;
  }
  .post-content {
    padding: 10px;
    text-align: center;
    background-color: #ccc;
  }
  a {
    color: black;
    text-decoration: none;      
  }
}
</style>