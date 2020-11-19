<template>
  <div class="container">
    <h2>
      Welcome to my Nuxt tutorial with Vercel  
    </h2> 
  </div>
</template>

<script lang="ts">

  export default {
    head() {
        return {
            title: "Index page for app",
            // meta data is good for SEO
            meta: [
                {
                    hid: "main_page",
                    name: "main_page",
                    content: "Main page for tutorial to use Nuxt with Vercel",
                }
            ],
        }
    }
  }
</script>

<style>

</style>
