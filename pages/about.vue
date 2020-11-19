<template>
    <div>
        <h1>My Nuxt Vercel App</h1>
        <p>Trying my first Nuxt App to be deployed on Vercel</p>
    </div>
</template>

<script>
export default {
    head() {
        return {
            title: "About the app",
            // meta data is good for SEO
            meta: [
                {
                    hid: "description",
                    name: "description",
                    content: "My tutorial to use Nuxt with Vercel",
                }
            ],
        }
    }
}
</script>

<style>

</style>