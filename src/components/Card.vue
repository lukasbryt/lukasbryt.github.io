<script>
export default {
    props: {
        content: { type: String, required: true },
    },
};
</script>
<template>
    <div class="mb-4 mx-3 ms-lg-5">
        <div class="card h-100">
            <img class="card-img-top" />
            <div class="card-body">
                <h3 v-html="content"></h3>
            </div>
        </div>
    </div>
</template>
<style scoped>
.card {
    background: var(--one);
    border-radius: 15px;
    border: none;
    box-shadow: 5px 6px 10px rgba(255, 174, 0, 0.39);
}
img{
    width: 100px !important;
}
</style>