<template>
    <div>
        <h1 class="title">{{msg}}</h1>
        <Banner></Banner>
        
    </div>
</template>

<script>
import Banner from '../components/Banner'
export default {
    name: 'HelloWorld',
    data () {
        return {
            msg: 'Hello World !!!'
        }
    },
    methods: {
        handleChange () {}
    },
    components: {
        Banner
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style>
    .title {
        text-align: center;
    }
</style>
