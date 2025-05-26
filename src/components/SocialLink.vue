<template>
    <button class="btn">
        <img class="btn__image" v-if="icon" :src="icon" alt="icon" />
        <p>TEXTO</p>
        <div class="btn__right"></div>
    </button>
</template>
<script lang="ts">
export default {
    name: "SocialLink",
    props: {
        icon: {
            type: String,
            required: false,
            default: "",
        },
    },
};
</script>

<style scoped lang="scss">
.btn {
    width: 100%;
    height: 60px;
    display: flex;
    flex-direction: row;
    align-items: center;
    text-align: center;

    gap: 4rem;
    padding: 0px 10px;

    border-radius: 10px;
    border: 1px solid #262626;

    transition: all 0.4s ease;
    &:hover {
        background-color: #ddd;
    }

    &__image {
        position: relative;
        left: 0;
        width: 40px;
        border-radius: 100px;
    }
    &__right {
        width: 40px;
    }
}
</style>
