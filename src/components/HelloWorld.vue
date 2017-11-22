<template>
    <div>
        <h1 class="title">{{msg}}</h1>
    </div>
</template>

<script>

export default {
    name: 'HelloWorld',
    data () {
        return {
            msg: 'vue-cli脚手架'
        }
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style>
    .title {
        text-align: center;
    }
</style>
