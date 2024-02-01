<script>

const ItemsHeader = [
    {
        text: 'Characters',
        url: '#',
        current: false,
    },
    {
        text: 'Comics',
        url: '#',
        current: true,
    },
    {
        text: 'Movies',
        url: '#',
        current: false,
    },
    {
        text: 'TV',
        url: '#',
        current: false,
    },
    {
        text: 'Games',
        url: '#',
        current: false,
    },
    {
        text: 'Collectibles',
        url: '#',
        current: false,
    },
    {
        text: 'Videos',
        url: '#',
        current: false,
    },
    {
        text: 'Fans',
        url: '#',
        current: false,
    },
    {
        text: 'News',
        url: '#',
        current: false,
    },
    {
        text: 'Shop',
        url: '#',
        current: false,
    },
];

export default {
    name: 'AppHeader',
    data() {
        return {
            ItemsHeader,
        };
    },
    methods: {
        selectedItem(index) {
            this.ItemsHeader.forEach((item, i) => {
                item.current = i === index;
            });


        }
    }
};
</script>


<template>
    <header>
        <div class="container">
            <img src="../assets/img/dc-logo.png" alt="Logo Dc comics">
            <ul>
                <li v-for="(item, index) in ItemsHeader" :key="item.text">
                    <a :href="item.url" :class="{ current: item.current }" @click="selectedItem(index)">{{ item.text
                    }}</a>
                </li>
            </ul>
        </div>
    </header>
</template>

<style scoped>
header {
    background-color: white;
}

div {
    height: 80px;
    display: flex;
    justify-content: space-between;
    align-items: center;
}

ul {
    display: flex;
    gap: 30px;
    list-style: none;
    font-weight: bold;
    text-transform: uppercase;
    font-size: small;
}

img {
    width: 70px;
}

a {
    text-decoration: none;
    color: black;
}

a.current {
    position: relative;
    text-decoration: none;
}

a.current::after {
    content: '';
    position: absolute;
    left: 0;
    bottom: -33px;
    width: 100%;
    height: 4px;
    background-color: dodgerblue;
}
</style>