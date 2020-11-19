<template>
    <div>
        This is my tutorial page    
    </div>    
</template>

<script>
import axios from "axios";

export default {
    data() {
        return {
            jokes: [],
        }
    },
    async created() {
        const config = {
            headers: {
                'Accept': 'application/json'
            }
        }
        try {
            const res = await axios.get('https://icanhazdadjoke.com/search', config);
            this.jokes = res.data.results;
        } catch (err) {
            console.log(err)
        }

        
    },
    head() {
        return {
            title: "Tutorial - Dad Jokes",
            // meta data is good for SEO
            meta: [
                {
                    hid: "tut",
                    name: "tut",
                    content: "Tut for things I'm trying",
                }
            ],
        }
    }
}
</script>

<style>

</style>