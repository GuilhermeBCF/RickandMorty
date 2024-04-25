<script setup>
import {ref} from 'vue'

let num = ref(0)

</script>

<template>
<nav class="navbar navbar-expand-lg navbar-dark bg-dark border-bottom border-body">
  <div class="container-fluid">
    <router-link class="navbar-brand" to="/">Rick and Morty</router-link>
    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNavAltMarkup" aria-controls="navbarNavAltMarkup" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarNavAltMarkup">
      <div class="navbar-nav">
        <router-link class="nav-link active" aria-current="page" to="/">Home</router-link>
        <router-link class="nav-link" to="/about">About</router-link>
      </div>
    </div>
  </div>
</nav>

<div class="main">
  <router-view></router-view>
</div>

<footer class="bg-dark text-light">
  <div> Unimar | ADS | {{ new Date().getFullYear() }}</div>
</footer>
</template>

<style>
footer{
  position: fixed;
  bottom:0;
  width:100%;
  display:flex;
  align-items: center;
  justify-content: center;
  height: 40px;
}
</style>