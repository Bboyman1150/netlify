<template>
    <nav class="navbar navbar-expand-lg navbar-dark bg-dark">
        <a class="navbar-brand" href="#">Navbar</a>
        <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNavAltMarkup"
            aria-controls="navbarNavAltMarkup" aria-expanded="false" aria-label="Toggle navigation">
            <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarNavAltMarkup">
            <div class="navbar-nav">
               
                <!-- <a class="nav-link" href="#">Home</a> -->
                <!-- <a class="nav-link" href="#">Movies</a> -->
                <router-link class="nav-link" to="/">Home</router-link>
                <router-link class="nav-link" to="/movies">Movies</router-link>

            </div>
        </div>
    </nav>
</template>

<script>
    export default {
        name:'Nav'

    }
</script>

<style scope>
    .navbar {padding: 25px}
</style>