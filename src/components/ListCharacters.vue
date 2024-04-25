<script setup>
    const character = defineProps(["name", "status", "species", "gender", "location", "image", "episode"])
</script>

<template>
    <div class="col-md-4">
        <div class="card mb-3 p-2">
            <img :src="character.image" class="card-img-top" height="100%" alt="...">
            <div class="card-body">
                <p class="card-title">Nome: {{ character.name }}</p>
                <p class="card-title">Status: {{ character.status }}</p>
                <p class="card-title">Espécie: {{ character.species }}</p>
                <p class="card-title">Gênero: {{ character.gender }}</p>
                <p class="card-title">Localização Atual: {{ character.location.name }}</p>
                <p class="card-title">Episódios: {{ character.episode.length }}</p>
            </div>
        </div>
    </div>
</template>