<template>
    <div>
        <h1 class="title">{{msg}}</h1>
        <Banner></Banner>
        <div class="bottom-btn">
            <el-button type="primary"><router-link class="link-btn" to="/home">开始你的操作</router-link><i class="el-icon-d-arrow-right el-icon--right"></i></el-button>
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
    .link-btn {
        display: inline-block;
        width: 100%;
        height: 100%;
    }
</style>
