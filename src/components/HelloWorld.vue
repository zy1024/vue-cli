<template>
    <div class="hello container">
        <h1 class="title">{{msg}}</h1>
        <Banner class="animated bounce"></Banner>
        <div class="bottom-btn">
            <router-link to="/home/123456" class="btn btn-info">开始你的操作</router-link>
            <button @click="clickFn" class="btn btn-primary">请求数据</button>
            <div class="row">
                <div class="col-lg-3 col-lg-offset-3">
                    <div class="bg-danger animated bounce">测试动画</div>
                    {{scrolled}}
                </div>
            </div>
            
        </div>
    </div>
</template>

<script>
import Banner from '../components/Banner'
import NewsData from '../../src/assets/data/news.js'
export default {
    name: 'HelloWorld',
    data () {
        return {
            msg: 'Hello World !!!',
            scrolled: ''
        }
    },
    methods: {
        clickFn() {
            console.log('引入js')
            console.log(NewsData)
        },
        handleScroll() {
            this.scrolled = window.scrollY
        }
    },
    mounted() {
        window.addEventListener('scroll', this.handleScroll)
    },
    components: {
        Banner
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="less" scope>
    .bottom-btn {
        margin-top: 20px;
        text-align: center;
    }
    .hello {
        height: 1000px;
        border: 1px solid #000;
        .title {
            color: red;
        }
    }
</style>
