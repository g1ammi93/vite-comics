<script>
export default {

}
</script>

<template>
    <main>
        <div class="container content">
            <h1>--Content goes Here--</h1>
        </div>
        <div class="main-menu">
            <h1 style="color: white">CICCIO</h1>
        </div>
    </main>
</template>

<style lang="scss" scoped>
@use '../assets/scss/_variables.scss' as variables;

main {
    background-color: black;
}

.content {
    height: 80px;
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
</style>