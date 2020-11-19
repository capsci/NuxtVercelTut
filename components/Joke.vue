<template>
    <nuxt-link :to="'tutorial/' + id">
        <div class="joke">
            {{ joke }}
        </div>
    </nuxt-link>
</template>

<script>
export default {
    name: 'Joke',
    props: ['joke', 'id']
}
</script>

<style>
.joke {
  padding: 1rem;
  border: 1px dotted #ccc;
  margin: 1rem 0;
}
</style>