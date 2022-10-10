<template>
    <nuxt-link :to="`/posts/${1}`" class="post-preview">
        <article>
          <div class="post-thumbnail" style="background-image: url('https://cdn.sabay.com/cdn/media.sabay.com/media/sabay-news/Sport-News/International-Sports/Freelancer-Sport/football(87)/6340122caf378_1665143340_medium.png');"></div>
          <div class="post-content">
            <h1>Post title</h1>
            <p>Post text</p>
          </div>
        </article>
    </nuxt-link>
</template>

<script>
export default {
    
}
</script>

<style lang="scss" scoped>
.home-page {
  .intro {
    height: 300px;
    position: relative;
    padding: 30px;
    box-sizing: border-box;
    background-position: center;
    background-size: cover;

    h1 {
      position: absolute;
      top: 10%;
      left: 5%;
      width: 90%;
      font-size: 1.5rem;
      color: black;
      background-color: rgb(211, 211, 211);
      padding: 10px;
      border-radius: 10px;
      box-shadow: 3px 3px 3px black;
      box-sizing: border-box;
      border: 1px solid black;
    }
  }
  .featured-posts {
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
}
@media (min-width: 850px) {
  .featured-posts {
    .post-preview {
      width: 400px;
      margin: 10px;
    }
  }
}
@media (min-width: 768px) {
  .home-page {
    .intro {
      h1 {
        font-size: 2rem;
      }
    }
  }
}
</style>