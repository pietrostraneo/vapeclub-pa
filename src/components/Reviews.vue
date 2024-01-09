<script>
import axios from 'axios'
export default {
    name: 'Reviews',
    data() {
        return {
            components: {
                axios
            }
        }
    },
    created() {
        axios.get("https://flynn.boolean.careers/exercises/api/random/mail").then((response) => {
            console.log(response.data.response)
        })
    }
}
</script>
<template lang="">
    <div>
        
    </div>
</template>
<style lang="scss" scoped>
@use '../styles/generals.scss';
</style>