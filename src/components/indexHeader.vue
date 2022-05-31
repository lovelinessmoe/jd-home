<template>
    <div class="header">
        <div class="w">
            <div class="logo">
                <a href=""> </a>
            </div>
            <div class="search">
                <search></search>
                <div class="hotwords_slide">
                    <slide height="16px" :pics="slideHotwords" :img=false ip="none" arrow="never"
                           :interval=1500></slide>
                </div>
                <NavItem :items="hotwords" class="hotwords"></NavItem>
            </div>
            <div class="navigation">
                <NavItem style="font-size: 20px" :items="items" :colors="color" fs="15px"></NavItem>
            </div>
            <div class="car">
                <el-button size="large" :icon="Briefcase">购物车</el-button>
            </div>
        </div>
    </div>
</template>

<script>

    import NavItem from './NavItem.vue';
    import search from "./search.vue";
    import Slide from './slide.vue';
    import {Briefcase} from '@element-plus/icons-vue'

    export default {
        data() {
            return {
                color: 'black',
                items: [
                    {
                        name: "秒杀",
                        url: ""
                    },
                    {
                        name: "优惠券",
                        url: ""
                    },
                    {
                        name: "PLUS会员",
                        url: ""
                    },
                    {
                        name: "品牌闪购",
                        url: ""
                    },
                    {
                        name: "拍卖",
                        url: ""
                    },
                    {
                        name: "京东家电",
                        url: ""
                    },
                    {
                        name: "京东超市",
                        url: ""
                    },
                    {
                        name: "京东生鲜",
                        url: ""
                    },
                    {
                        name: "京东国际",
                        url: ""
                    },
                    {
                        name: "京东云",
                        url: ""
                    },

                ],
                slideHotwords: [
                    {
                        url: "车品特惠购",
                        Path: ""
                    },
                    {
                        url: "京造运动会",
                        Path: ""
                    },
                    {
                        url: "抢健康五折",
                        Path: ""
                    }
                ],
                hotwords: [

                    {
                        name: "拉面说",
                        Path: ""
                    },
                    {
                        name: "奇异果",
                        Path: ""
                    },
                    {
                        name: "健康好物",
                        Path: ""
                    },
                    {
                        name: "沃尔玛",
                        Path: ""
                    },
                    {
                        name: "reno6",
                        Path: ""
                    },
                    {
                        name: "车品特惠",
                        Path: ""
                    },
                    {
                        name: "蓝月亮",
                        Path: ""
                    },
                    {
                        name: "运动会",
                        Path: ""
                    },
                ],
                Briefcase
            }
        },
        name: "indexheader",
        components: {
            search,
            NavItem,
            Slide,

        },
    };
</script>

<style lang="less" scoped>
    .navigation {
        color: black;
    }

    .hotwords_slide {
        color: red;
        width: 70px;
        /* display: inline-block; */
        float: left;
        font-size: 12px;
    }

    .header {
        height: 140px;
        background-color: #fff;
        border-bottom: 1px solid #ddd;
        margin-bottom: 10px;
    }

    .header .w {
        position: relative;
    }

    .logo {
        position: absolute;
        background-image: url("https://misc.360buyimg.com/mtd/pc/index_2019/1.0.0/assets/sprite/header/sprite.png");
        left: 0;
        top: 10px;
        width: 190px;
        height: 120px;
    }

    .search {
        position: absolute;
        top: 30px;
        /* background-color: green; */
        left: 300px;
        width: 550px;
        /* height: 50px; */
    }

    .car {
        position: absolute;
        right: 200px;
        /*background-color: pink;*/
        top: 30px;
        height: 40px;
        width: 100px;
    }

    .navigation {
        position: absolute;
        top: 120px;
        left: 300px;
        // background-color: rgb(183, 203, 123);
    }

    .hotwords {
        /*float: left;*/
        color: var(--darkgray);
        font-size: 12px;
    }
</style>
