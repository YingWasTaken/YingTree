<template>
    <section>
        <Avatar :image="this.image" />
        <Name :name="this.name" :subtitle="this.subtitle" />
        <div><SocialLink icon="/images/default.jpg" btnText="TEXTOBTN" /></div>
    </section>
</template>

<script lang="ts">
import Avatar from "/src/components/Avatar.vue";
import Name from "/src/components/Name.vue";
import SocialLink from "/src/components/SocialLink.vue";

export default {
    name: "App",
    components: {
        Avatar,
        Name,
        SocialLink,
    },
    data() {
        return {
            image: "/images/default.jpg",
            name: "Pablo",
            subtitle: "Autistic",
        };
    },
};
</script>

<style scoped lang="scss"></style>
