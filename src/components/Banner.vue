<template>
    <div>
        <el-row>
            <el-col :span="12" :offset="6">
                <el-carousel :interval="4000" type="card" height="180px">
                    <el-carousel-item v-for="img in bannerImg">
                        <div class="banner_img"><img :src="img.url"></div>
                    </el-carousel-item>
                </el-carousel>
                <div class="bottom-btn">
                    <el-button type="primary">开始你的操作<i class="el-icon-d-arrow-right el-icon--right"></i></el-button>
                </div>
            </el-col>
        </el-row>     
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
    .bottom-btn {
        margin-top: 20px;
        text-align: right;
    }
</style>