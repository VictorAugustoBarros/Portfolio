<template>
    <div class="navbar">
        <v-row>
            <v-col cols="8"></v-col>
            <v-col cols="4">
                <router-link class="no-underline" to="/">PROJETOS</router-link>
            </v-col>
        </v-row>
    </div>
</template>

<script>
export default {
    name: "NavBar",
}
</script>

<style>

.no-underline {
    text-decoration: none;
    color: inherit;
    color: gray
}

.navbar {
    display: flex;
    justify-content: center;
    align-items: center;
    height: 10vh;
    /* opacity: 0.9; */
}
</style>