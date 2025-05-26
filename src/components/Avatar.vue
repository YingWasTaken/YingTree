<template>
    <img class="avatar" :src="this.image" alt="" />
</template>

<script lang="ts">
export default {
    name: "Avatar",
    props: {
        image: {
            type: String,
            required: false,
            default: "/images/default.jpg",
        },
    },
};
</script>

<style scoped lang="scss">
.avatar {
    width: 150px;
    border-radius: 100px;
}
</style>
