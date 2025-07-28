<template>
    <div class="post">
        <div>
            <div><strong>Title </strong>{{ post.title }}</div>
            <div><strong>Body </strong>{{ post.body }}</div>
        </div>


        <div class="post__buttons">
            <my-button
            @click="$emit('remove', post)">
                To delete
            </my-button>
        </div>

    </div>
</template>
<script>

export default {

    props: {
        post: {
            type: Object,
            required: true,
        }
    }
}

</script>

<style scoped>
.post {
    padding: 15px;
    border: 1px solid teal;
    margin-top: 15px;
    display: flex;
    align-items: center;
    justify-content: space-between;
}
</style>