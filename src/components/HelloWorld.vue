<template>
    <div>
        <h1 class="title">{{msg}}</h1>
        <Banner></Banner>
        <div class="bottom-btn">
            <router-link to="/home" class="btn btn-info">开始你的操作</router-link>
            <button @click="clickFn" class="btn btn-primary">请求数据</button>
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
        clickFn() {
            this.$http({
                url: '/api/AppServer/n/article/article?type=carGuide',
                method: 'post'
            })
            .then(function(res){
                console.log(res)
            })
        }
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
