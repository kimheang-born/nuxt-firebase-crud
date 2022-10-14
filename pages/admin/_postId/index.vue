<template>
    <div class="admin-post-page">
        <section class="update-form">
            <AdminPostForm :post="loadedPost"/>
        </section>
    </div>
</template>

<script>
import AdminPostForm from "@/components/Admin/AdminPostForm";

export default {
    components: {
        AdminPostForm,
    },
    data() {
        return {
            loadedPost: {
                author: 'Kimheang',
                title: 'My title',
                content: 'My content',
                thumbnailLink: 'https://cdn.sabay.com/cdn/media.sabay.com/media/sabay-news/Sport-News/International-Sports/soccer/Soccer54/Soccer144/Soccer212/634386e3ea970_1665369780_large.jpg',
            }
        }
    },
}
</script>

<style lang="scss" scoped>
.update-form {
    width: 90%;
    margin: 20px auto;
}
@media (min-width: 768px) {
    .update-form {
        width: 500px;
    }
}
</style>
