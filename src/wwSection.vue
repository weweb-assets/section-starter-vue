<template>
    <div class="my-section">
        <h1>{{ content.title }}</h1>
        <wwLayout class="drop-zone" path="list"></wwLayout>
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
        list: [],
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
    .drop-zone {
        display: block;
        min-height: 300px;
        width: 50%;
        margin: 18px;
        padding: 18px;
        background-color: #fafafa;
        border: 1px solid #535353;
    }
}
</style>
