<script>
import BookCard from './books/BookCard.vue';

export default {
    name: 'AppMain',
    props: {
        books: Array
    },
    components: { BookCard }
}
</script>

<template>
    <main>
        <div class="container content">
            <div class="card-container">
                <BookCard v-for="book in books" :key="book.series" :image="book.thumb" :title="book.series" />

            </div>

        </div>
        <div class="flex-center">
            <button>SIGN-UP NOW!</button>
        </div>
        <div class="main-menu">

        </div>
    </main>
</template>

<style lang="scss" scoped>
@use '../assets/scss/_variables.scss' as variables;

main {
    background-color: black;
}

.content {
    min-height: 219px;
    display: flex;
    align-items: center;
}

h1 {
    color: white;
    font-size: 23px;
}

.main-menu {
    background-color: variables.$color;
    height: 120px;

}

.card-container {
    display: flex;
    flex-wrap: wrap;
    margin: 30px 0;
}

.book-card {
    flex-basis: 15%;
}

button {
    padding: 10px;
    background-color: variables.$color;
    color: white;
    border: 1px solid variables.$color;
    cursor: pointer;
    margin-bottom: 15px;
    text-align: center;
}

.flex-center {
    display: flex;
    justify-content: center;
}
</style>