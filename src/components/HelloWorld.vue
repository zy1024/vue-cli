<template>
    <div>
        <h1 class="title">{{msg}}</h1>
        <Banner></Banner>
        <div class="bottom-btn">
            <router-link to="/home">开始你的操作</router-link>
        </div>
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
<style scope>
    .title {
        text-align: center;
    }
    .bottom-btn {
        margin-top: 20px;
        text-align: center;
    }
</style>
