<script>
export default {
    props: {
        title: { type: String, required: true },
        text: { type: String, required: true },
        img: { type: String, required: true },
        link: { type: String, required: true },
        linktitle: { type: String, required: true }
    },
};
</script>
<template>
    <a target="_blank" :href="link" class="card-link">
        <div class="card m-sm-4" style="width: 18rem;">
            <img :src="img"
                class="card-img-top">
            <div class="card-body">
                <h3 class="card-title">{{ title }}</h3>
                <p class="card-text">{{ text }}</p>
            </div>
        </div>
    </a>
</template>
<style scoped>
div {
    font-family: Ubuntu, sans-serif;
}
img{
    width: 288px;
    height: 173;
}
.card {
    background-color: var(--three);
    border-radius: 15px;
    border: none;
    transition: 1s;
}
.card:hover {
  transform: scale(1.05);
  transition: 0.2s;
  box-shadow: 5px 5px 15px rgba(0, 0, 0, 0.329);
}
.card-img-top {
    border-radius: 15px 15px 0 0;
    padding: 8px;
}

h3 {
    font-weight: 900;
    color: var(--two);
}
p{
    color: var(--two);
    font-weight: 400;
    font-size: 18px;
}

a {
    padding: 10px 50px;
    border-radius: 15px;
    color: var(--three);
    text-decoration: none;
    font-weight: 900;
}
</style>