<template>

    <div>
        <div class="post" v-for="post in posts">
            <div><strong>Title </strong>{{ post.title }}</div>
            <div><strong>Body </strong>{{ post.body }}</div>

        </div>

    </div>
</template>

<script>
export default {
    data() {
        return {
            posts: [
                { id: 1, title: 'javascript', body: ' describing' },
                { id: 2, title: ' javascript', body: ' describing 2' },
                { id: 3, title: ' javascript', body: ' describing 3' },
            ]
        }
    },
    methods: {
        addLike() {

        }
    }
}

</script>

<style>
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;

    .post {
        padding: 15px;
        border: 1px solid teal;
        margin-top: 15px;
    }
}
</style>