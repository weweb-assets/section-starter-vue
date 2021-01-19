<template>
    <div class="my-section">
        <h1>{{ content.title }}</h1>
        <p>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et
            dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex
            ea commodo consequat.
        </p>
    </div>
</template>

<script>
export default {
    name: '__COMPONENT_NAME__',
    props: {
        content: {
            type: Object,
        },
    },
    wwDefaultContent: {
        title: 'My title',
    },
};
</script>

<style lang="scss" scoped>
.my-section {
    display: flex;
    flex-direction: column;
    justify-content: center;
    min-height: 200px;
    h1 {
        font-size: 32px;
    }
    p {
        margin-top: 12px;
    }
}
</style>
