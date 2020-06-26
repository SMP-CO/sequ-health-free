<template>
        <b-navbar class="nav" fixed-top>
            <template slot="brand">
                <b-navbar-item tag="a" href="https://sequ-suite.com">
                    <img src="img/suitelogo.png"
                         alt="SEQu-SUITE">
                </b-navbar-item>
            </template>
            <template slot="end">
                <b-navbar-item tag="a" href="https://sequ-suite.com">Go to sequ-suite.com →</b-navbar-item>
            </template>
        </b-navbar>
</template>

<script>
    import BNavbar from "buefy/src/components/navbar/Navbar";
    import BNavbarItem from "buefy/src/components/navbar/NavbarItem";
    export default {
        name: "Nav",
        components: {BNavbarItem, BNavbar}
    }
</script>

<style scoped>
    .nav {
        border-bottom: solid 1px #262626;
    }
</style>