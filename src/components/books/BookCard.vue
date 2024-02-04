<script>
export default {
    name: 'BookCard',
    props: {
        image: String,
        title: String
    }
}
</script>

<template>
    <div class="book-card">

        <img :src="image" :alt="title">
        <h3>{{ title }}</h3>
    </div>
</template>

<style scoped>
.book-card {
    padding: 20px;
    background-color: transparent;
    border: lightblue;
    height: 180px;
    width: 180px;
    margin-bottom: 10px;


}

h3 {
    color: white;
    font-size: 12px;
    margin-top: 5px;
    font-weight: normal;
    text-transform: uppercase;
    cursor: pointer;
}

img {
    display: block;
    width: 100%;
    height: 100%;
    object-fit: cover;
    object-position: top;
    cursor: pointer;

}
</style>