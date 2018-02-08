<template>
    <div>
        lsjgsldjglsag   
    </div> 
</template>

<script>
    export default {
        data () {
            return {
                bannerImg: [
                    {
                        "name": "banner1",
                        "url": "/static/images/banner1.png"
                    },
                    {
                        "name": "banner2",
                        "url": "/static/images/banner2.png"
                    },
                    {
                        "name": "banner3",
                        "url": "/static/images/banner3.png"
                    }
                ]
            }
        },
        methods: {

        }
    }
</script>

<style scope>
    .el-carousel__item .banner_img img {
        width: 100%;
    }
    .el-carousel__item:nth-child(2n) {
        background-color: #99a9bf;
    }
  
    .el-carousel__item:nth-child(2n+1) {
        background-color: #d3dce6;
    } 
</style>