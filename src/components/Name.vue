<template>
    <div class="name-section">
        <h1 class="name-section__name">@{{ this.name }}</h1>
        <h2 class="name-section__subtitle">{{ this.subtitle }}</h2>
    </div>
</template>
<script lang="ts">
export default {
    name: "Name",
    props: {
        name: {
            type: String,
            required: false,
            default: "name",
        },
        subtitle: {
            type: String,
            required: false,
        },
    },
};
</script>
<style scoped lang="scss">
.name-section {
    margin-bottom: 20px;
    margin-top: 10px;
    &__name {
        color: white;
        font-size: 24px;
        text-transform: uppercase;
    }

    &__subtitle {
        color: whitesmoke;
        font-size: 14px;
        text-transform: uppercase;
    }
}
</style>
