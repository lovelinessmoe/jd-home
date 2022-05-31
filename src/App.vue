<script>
    import Home from "./components/Home.vue";

    export default {
        components: {Home}
    }
</script>

<template>
    <Home></Home>
</template>


<style lang='less'>
    @darkgray: rgb(153, 153, 153);
    * {
        margin: 0;
        padding: 0;
        font: 12px/1.5 Microsoft YaHei, Heiti SC, tahoma, arial, Hiragino Sans GB,
        "\5B8B\4F53", sans-serif;
    }

    :root {
        --gray: rgb(227, 228, 229);
        --red: rgb(225, 37, 27);
        --darkgray: rgb(153, 153, 153);
        --gray-bg: rgb(244, 244, 244);
    }

    a {
        text-decoration: none;
        color: inherit;
        font-size: inherit;
    }

    *:hover {

    }

</style>

