<template>
    <div class="single-post-page">
        <section class="post">
            <h1 class="post-title">Title of post</h1>
            <div class="post-details">
                <div class="post-detail">Last updated on XXX</div>
                <div class="post-detail">Written by Name</div>
            </div>
            <p class="post-content">Content of post</p>
        </section>
        <section class="post-feedback">
            <p>Let me know what you about the post, send a mail to <a href="mailto:john.doe@gmail.com">john.doe@gmail.com</a>.</p>
        </section>
    </div>
</template>

<script>
export default {
    
}
</script>

<style lang="scss" scoped>
.single-post-page {
    padding: 30px;
    text-align: center;
    box-sizing: border-box;

    .post {
        width: 100%;

        .post-title {
            margin: 0;
        }

        .post-details {
            padding: 10px;
            box-sizing: border-box;
            border-bottom: 3px solid #ccc;
            display: flex;
            justify-content: center;
            align-items: center;
            flex-direction: column;
        }
        .post-detail {
            color: rgb(88, 88, 88);
            margin: 0 10px;
        }
    }

    .post-feedback {
        a {
            color: red;
            text-decoration: none;

            &:hover,
            &:active {
                color: salmon;
            }
        }
    }
}

@media (min-width: 768px) {
    .post {
        width: 600px;
        margin: auto;

        .post-details {
            flex-direction: row;
        }
    }
}

</style>