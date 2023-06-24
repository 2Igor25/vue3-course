<template>
    <div>
        <div>
            <button @click="addLike">Like</button>
            <button @click="addDislike">DisLike</button>
        </div>
        <div>Количество лайков: <strong>{{ likes }}</strong></div>
        <div>Количество дизлайков: <strong>{{dislike }}</strong></div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            likes: 0,
            dislike: 0,
        }
    },
    methods: {
        addLike() {
            this.likes += 1;
        },
        addDislike() {
            this.dislike += 1;
        }
    }
}
</script>

<style>
</style>