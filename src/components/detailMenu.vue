<style lang="scss" scoped>
    .active{
        width: 674px!important; ;
        transition:width 1s;
        -moz-transition:width 1s; /* Firefox 4 */
        -webkit-transition:width 1s; /* Safari and Chrome */
        -o-transition:width 1s; /* Opera */
    }
    .main-nav {
        left: 0;
        width: 186px;
        position: absolute;
        #j-mainSortList{
            display: none;
        }
        .sortList {
            position: relative;
            zoom: 1;
            z-index: 10;
            height: 582px;

            .list{
                .li1 i {
                    background-position-y: 1px;
                }
                li {
                    background-color: #3b3a3b;
                    background-color: rgba(59, 58, 59, .8);
                    padding-left: 19px;
                    padding-top: 12px;
                    padding-bottom: 11px;
                    cursor: pointer;
                    border-bottom: 1px solid rgba(255, 255, 255, .15);
                    position: relative;
                    zoom: 1;
                    .sort1 {
                        font-size: 14px;
                        color: #fff;
                        line-height: 20px;
                        i {
                            display: inline-block;
                            width: 18px;
                            height: 20px;
                            vertical-align: sub;
                            background: url(//cdn2.duoduoyin.com/static/ddy-common/images/icon/ico-nav_da13042.png) no-repeat;
                            background-position-x: 0;
                            margin-right: 10px;
                        }
                        a {
                            font-weight: 700;
                            line-height: 26px;
                        }
                    }
                    .sort2 {
                        font-size: 12px;
                        color: #fff;
                        line-height: 19px;
                        a {
                            padding-right: 10px;
                        }
                    }
                }
            }
            .subsort {
                width: 1104px;
                height: 582px;
                position: absolute;
                zoom: 1;
                top: 0;
                left: 186px;
                cursor: default;
                z-index: 5;
                /* display: none; */
                .subwrap {
                    width: 1004px;
                    height: 582px;
                    .subad {
                        width: 330px;
                        height: 582px;
                        background-color: #f5f5f5;
                        float: left;
                        display: inline;
                        position: relative;
                        zoom: 1;
                        z-index: 2;
                        margin-left: -247px;
                        img {
                            width: 330px;
                            height: 582px;
                        }
                    }
                    .subbox {
                        width: 0px;
                        height: 582px;
                        float: left;
                        display: inline;
                        position: relative;
                        zoom: 1;
                        z-index: 3;
                        overflow: hidden;
                        background-color: #fff;
                        .boxc {
                            width: 674px;
                            height: 582px;
                            position: absolute;
                            zoom: 1;
                            right: -20px;
                            .subtitle {
                                float: left;
                                width: 106px;
                                color: #4d4d4d;
                                font-size: 14px;
                                padding: 15px 0 20px;
                                span {
                                    font-weight: 700;
                                    line-height: 35px;
                                    position: relative;
                                    zoom: 1;
                                }
                            }
                            .sublist {
                                width: 480px;
                                float: left;
                                padding: 15px 0 20px;
                                border-bottom: 1px dashed #dcdcdc;
                                a {
                                    display: inline-block;
                                    color: #8d8d8d;
                                    white-space: normal;
                                    word-wrap: break-word;
                                    padding-right: 18px;
                                    font-size: 14px;
                                    vertical-align: top;
                                    overflow: visible;
                                    line-height: 35px;
                                }
                                .crown-item {
                                    position: relative;
                                    zoom: 1;
                                }
                            }
                        }
                    }
                }
            }

        }
        .allsort {
            background: url(//cdn2.duoduoyin.com/static/ddy-common/images/index/sortbg_ca9ca72.png) 0 0 no-repeat;
            height: 41px;
            font-size: 16px;
            padding-left: 19px;
            line-height: 41px;
            color: #fff;
            position: relative;
            zoom: 1;
            z-index: 10;
            i {
                display: inline-block;
                width: 15px;
                height: 12px;
                margin-right: 11px;
                background: url(//cdn2.duoduoyin.com/static/ddy-common/images/icon/ico-sort_a2fefc4.png) 0 0 no-repeat;
            }
        }
    }
</style>
<template>
    <div class="main-nav" @mouseenter="enterStyleone('main-nav')" @mouseleave='leaveStyleone("main-nav")'>
        <div class="allsort"  ><i></i><span>印品分类</span></div>
        <div class="sortList" id="j-mainSortList">
            <ul class="list">
                <li class="li1 j-li" data-id="sort1" @mouseenter="enterStyle" @mouseleave='leaveStyle'  data-adlink="http://www.duoduoyin.com/mingpianLuxury.html"
                    data-adimg="//image.duoduoyin.com/uploads/aid/20180319/180319033807f68df16f93.jpg">
                    <div class="sort1"><i></i><a target="_blank" href="/mingpian.html">名片</a></div>
                    <div class="sort2"><a target="_blank" href="/goods/1.html">铜版纸</a><a target="_blank" href="/goods/173.html">安格纸</a><a
                            target="_blank" href="/goods/226.html">丽芙纸</a><br><a target="_blank" href="/goods/45.html">黑卡纸</a><a
                            target="_blank" href="/goods/168.html">欧纯棉纸</a><a target="_blank" href="/zhiyang.html">纸样</a></div>
                </li>
                <li class="li2 j-li" data-id="sort9" data-adlink="http://www.duoduoyin.com/toteBag.html"
                    data-adimg="//image.duoduoyin.com/uploads/aid/20180319/180319033937f69396d653.jpg">
                    <div class="sort1"><i></i><a target="_blank" href="/toteBag.html">手提袋</a></div>
                    <div class="sort2"><a target="_blank" href="/goods/292.html">白卡纸</a><a target="_blank" href="/goods/294.html">牛皮纸</a><a
                            target="_blank" href="/toteBag.html#fabric">无纺布</a><br><a target="_blank" href="/goods/298.html">帆布袋</a><a
                            target="_blank" href="/goods/297.html">塑料袋</a><a target="_blank" href="/toteBag.html#spot">现货</a></div>
                </li>
                <li class="li3 j-li" data-id="sort2" data-adlink="http://www.duoduoyin.com/huace.html"
                    data-adimg="//image.duoduoyin.com/uploads/aid/20180319/180319033844f690411d62.jpg">
                    <div class="sort1"><i></i><a href="javascript:;">宣传</a></div>
                    <div class="sort2"><a target="_blank" href="/xuanchuandan.html">宣传单</a><a target="_blank" href="/huace.html">画册</a><a
                            class="ar" target="_blank" href="/buganjiaotie.html">不干胶贴</a><br><a target="_blank"
                                                                                                href="/yilabao.html">易拉宝</a><a
                            target="_blank" href="/zheye.html">折页</a><a target="_blank" href="/wenhuashan.html">文化衫</a></div>
                </li>
                <li class="li4 j-li" data-id="sort3" data-adlink="http://www.duoduoyin.com/goods/274.html"
                    data-adimg="//image.duoduoyin.com/uploads/aid/20180319/180319033901f6915e9892.jpg">
                    <div class="sort1"><i></i><a href="javascript:;">办公</a></div>
                    <div class="sort2"><a target="_blank" href="/gongzuozheng.html">工作证</a><a target="_blank"
                                                                                              href="/goods/75.html">信纸</a><a
                            target="_blank" href="/goods/108.html">信封</a><a target="_blank" href="/goods/60.html">便签</a><br><a
                            target="_blank" href="/jishiben.html">记事本</a><a target="_blank" href="/goods/74.html">文件袋</a><a
                            target="_blank" href="/goods/76.html">纸杯</a></div>
                </li>
                <li class="li5 j-li" data-id="sort7" data-adlink="http://www.duoduoyin.com/activity/foodBeverage.html"
                    data-adimg="//image.duoduoyin.com/uploads/aid/20180319/180319034430f6a5e98582.png">
                    <div class="sort1"><i></i><a href="/activity/foodBeverage.html" target="_blank">餐饮印品</a></div>
                    <div class="sort2"><a target="_blank" href="/goods/305.html">订餐卡</a><a class="ar" target="_blank"
                                                                                           href="/goods/311.html">不干胶</a><a
                            target="_blank" href="/goods/306.html">DM单</a><br><a target="_blank" href="/goods/303.html">餐巾纸</a><a
                            target="_blank" href="/goods/309.html">垫餐纸</a><a target="_blank" href="/goods/312.html">餐盒腰封</a></div>
                </li>
                <li class="li6 j-li" data-id="sort8" data-adlink="http://www.duoduoyin.com/kuaiyin.html"
                    data-adimg="//image.duoduoyin.com/uploads/aid/20180319/180319033925f692decbd6.jpg">
                    <div class="sort1"><i></i><a href="javascript:;">速印</a></div>
                    <div class="sort2"><a target="_blank" href="/goods/267.html">项目书</a><a target="_blank" href="/goods/268.html">投标书</a><a
                            target="_blank" href="/goods/263.html">VI手册</a><br><a target="_blank" href="/goods/266.html">培训书</a><a
                            target="_blank" href="/zhaopianshu.html">相册书</a><a target="_blank" href="/goods/265.html">产品手册</a></div>
                </li>
            </ul>
            <div class="subsort" @mouseenter="enterStyleone('subsort')" @mouseleave='leaveStyleone("subsort")' id="j-mainSubsort" style="display: none;">
                <div class="subwrap">
                    <div class="subbox j-subbox" >
                        <div class="boxc j-box">
                            <div class="subtitle"><a target="_blank" href="/toteBag.html#classic"><span>经典手提袋</span></a></div>
                            <div class="sublist"><a target="_blank" href="/goods/292.html" class="hot-item">白卡纸手提袋</a> <a
                                    target="_blank" href="/goods/293.html">铜版纸手提袋</a> <a target="_blank" href="/goods/294.html">牛皮纸手提袋</a>
                                <a target="_blank" href="/goods/295.html">白牛皮纸手提袋</a></div>
                            <div class="subtitle"><a target="_blank" href="/toteBag.html#fabric"><span>无纺布手提袋</span></a></div>
                            <div class="sublist"><a target="_blank" href="/goods/299.html">平口无纺布手提袋</a> <a target="_blank"
                                                                                                           href="/goods/300.html"
                                                                                                           class="hot-item">立体无纺布手提袋</a>
                                <a target="_blank" href="/goods/301.html">船型无纺布手提袋</a> <a target="_blank" href="/goods/302.html">折叠无纺布手提袋</a>
                            </div>
                            <div class="subtitle"><a target="_blank" href="/toteBag.html#other"><span>其他手提袋</span></a></div>
                            <div class="sublist"><a target="_blank" href="/goods/298.html">帆布手提袋</a> <a target="_blank"
                                                                                                        href="/goods/297.html">塑料手提袋</a>
                                <a target="_blank" href="/goods/296.html">船型手提袋</a></div>
                            <div class="subtitle"><a target="_blank" href="/toteBag.html#spot"><span>现货手提袋</span></a></div>
                            <div class="sublist"><a target="_blank" href="/goods/291.html" class="hot-item">彩色牛皮纸手提袋</a></div>
                        </div>
                    </div>
                    <div class="subad j-subad" style="margin-left: 0px;"><a href="http://www.duoduoyin.com/toteBag.html"><img
                            src="//image.duoduoyin.com/uploads/aid/20180319/180319033937f69396d653.jpg"></a></div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        name: "listmenu",
        methods:{
            enterStyleone(className){
                $("#j-mainSortList").css({'display':'block'})
                console.log(2222)
            },
            leaveStyleone(className){
                $("#j-mainSortList").css({'display':'none'})
                console.log(4444)
            },
            enterStyle(){
                $("#j-mainSubsort").css({'display':'block'})
                $(".j-subbox").addClass('active')
            },
            leaveStyle(){
                $("#j-mainSubsort").css({'display':'none'})
                $(".j-subbox").removeClass('active')
            }

        }
    }
</script>

