<template>
    <div id="home">
        home

        <div>
            打印参数: {{$route.params}}
            <button @click="test($route.params)">click me</button>
        </div>
    </div>
</template>

<script>
    export default {
        data () {
            return {

            }
        },
        methods: {
            test(params) {
                console.log(params)
            }
        }
    }
</script>

<style>
    body {
        margin: 0;
    }
    .el-header, .el-footer {
        background-color: #B3C0D1;
        color: #333;
        text-align: center;
        line-height: 60px;
    }
  
    .el-aside {
        background-color: #D3DCE6;
        color: #333;
        text-align: center;
        line-height: 200px;
    }
      
    .el-main {
        background-color: #E9EEF3;
        color: #333;
        text-align: center;
        min-height: 500px;
    }
           
</style>