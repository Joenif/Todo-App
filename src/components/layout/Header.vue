<template>
  <div>
    <nav class="navbar navbar-expand-md navbar-dark navbar-laravel">
        <div class="container">
            <router-link :to="{name: 'Home'}" class="navbar-brand">My To-Dos</router-link>
            <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
            </button>

            <div class="collapse navbar-collapse" id="navbarSupportedContent">
                <!-- Left Side Of Navbar -->
                <ul class="navbar-nav mr-auto"></ul>
                <!-- Right Side Of Navbar -->
                <ul class="navbar-nav ml-auto">
                    <li class="nav-link"> Hi, {{user}}</li>
                </ul>
            </div>
        </div>
    </nav>
  </div>
</template>

<script>
export default {
    name: "Header",
    props: ["user"]
}
</script>

<style>

</style>