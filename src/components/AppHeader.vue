<template>
     <nav class="navbar navbar-dark bg-dark">
        <div class="container-fluid">
            <a href="#" class="navbar-brand">Marvel</a>
            <form class="d-flex">
                <input type="search" 
                placeholder="Search" 
                aria-label="Search" 
                class="form-control me-2"
                v-model.trim="search"
                @input="changeSearch(search)">
                <button type="reset" class="btn btn-outline-light">
                    Search
                </button>
            </form>
        </div>
    </nav>
</template>

<script>
    export default {
        name: "AppHeader",
        props: ["changeSearch"],
        data() {
            return {
                search:'',
            }
        },
    }
</script>

<style scoped>

</style>
