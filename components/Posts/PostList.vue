<template>
    <section class="post-list">
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
            previewText="This is my text 2."
        />
    </section> 
</template>

<script>
import PostPreview from "@/components/Posts/PostPreview"

export default {
    components: {
      PostPreview,
    }
}
</script>

<style lang="scss" scoped>
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