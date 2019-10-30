<template>
    <div>
        <Header></Header>
        <div class="gallery-wrap">
            <div class="col1">
                <a class="portfolio-box zoom-effect" href="/picture1">
					<img src="../img/image19.jpg" class="img-responsive" alt="">
					<div class="portfolio-box-caption"><div class="portfolio-box-caption-content"></div></div>
				</a>
                <a class="portfolio-box zoom-effect" href="/picture2">
					<img src="../img/image20.jpg" class="img-responsive" alt="">
					<div class="portfolio-box-caption"><div class="portfolio-box-caption-content"></div></div>
				</a>
                <a class="portfolio-box zoom-effect" href="/picture3">
					<img src="../img/image21.jpg" class="img-responsive" alt="">
					<div class="portfolio-box-caption"><div class="portfolio-box-caption-content"></div></div>
				</a>
            </div>
            <div class="col2">
                <a class="portfolio-box zoom-effect" href="/picture4">
					<img src="../img/image22.jpg" class="img-responsive" alt="">
					<div class="portfolio-box-caption"><div class="portfolio-box-caption-content"></div></div>
				</a>
                <a class="portfolio-box zoom-effect" href="/picture5">
					<img src="../img/image23.jpg" class="img-responsive" alt="">
					<div class="portfolio-box-caption"><div class="portfolio-box-caption-content"></div></div>
				</a>
                <a class="portfolio-box zoom-effect" href="/picture6">
					<img src="../img/image24.jpg" class="img-responsive" alt="">
					<div class="portfolio-box-caption"><div class="portfolio-box-caption-content"></div></div>
				</a>
                <a class="portfolio-box zoom-effect" href="/picture7">
					<img src="../img/image25.jpg" class="img-responsive" alt="">
					<div class="portfolio-box-caption"><div class="portfolio-box-caption-content"></div></div>
				</a>
            </div>
            <div class="col3">
                <a class="portfolio-box zoom-effect" href="/picture">
					<img src="../img/image26.jpg" class="img-responsive" alt="">
					<div class="portfolio-box-caption"><div class="portfolio-box-caption-content"></div></div>
				</a>
                <a class="portfolio-box zoom-effect" href="/picture9">
					<img src="../img/image27.jpg" class="img-responsive" alt="">
					<div class="portfolio-box-caption"><div class="portfolio-box-caption-content"></div></div>
				</a>
                <a class="portfolio-box zoom-effect" href="/picture10">
					<img src="../img/image28.jpg" class="img-responsive" alt="">
					<div class="portfolio-box-caption"><div class="portfolio-box-caption-content"></div></div>
				</a>
            </div>
        </div>
        <Footer></Footer>
    </div>
</template>

<script>
import Header from './Header.vue';
import Footer from './Footer.vue';

export default {
    components: {
        Header: Header,
        Footer: Footer,
    }
}
</script>

<style scoped>
.gallery-wrap {display: flex;justify-content: space-between;max-width: 1200px;margin: 70px auto;}
.col1, .col2, .col3 {max-width: 380px;}
.portfolio-box {display: block;position: relative;margin: 0 auto 30px;overflow: hidden;}
.portfolio-box:before{z-index:1;content:"";position:absolute;left:0;right:0;top:0;bottom:0;border-top:12px solid #131313;border-bottom:12px solid #131313;transform:scale(0,1);-moz-transform:scale(0,1);-webkit-transform:scale(0,1);-ms-transform:scale(0,1);transition:all 0.4s ease-in-out 0s;-moz-transition:all 0.4s ease-in-out 0s;-webkit-transition:all 0.4s ease-in-out 0s;}
.portfolio-box:after{z-index:1;content:"";position:absolute;left:0;right:0;top:0;bottom:0;border-left:12px solid #131313;border-right:12px solid #131313;transform:scale(1,0);-moz-transform:scale(1,0);-webkit-transform:scale(1,0);-ms-transform:scale(1,0);transition:all 0.4s ease-in-out 0s;-moz-transition:all 0.4s ease-in-out 0s;-webkit-transition:all 0.4s ease-in-out 0s;}
.portfolio-box:hover:before{transform:scale(1,1);-moz-transform:scale(1,1);-webkit-transform:scale(1,1);-ms-transform:scale(1,1);}
.portfolio-box:hover:after {transform:scale(1,1);-moz-transform:scale(1,1);-webkit-transform:scale(1,1);-ms-transform:scale(1,1);}
.portfolio-box.zoom-effect img{transition: 0.5s ease;width: 100%;}
.portfolio-box:hover.zoom-effect img{transform:scale(1.1)}
.portfolio-box .portfolio-box-caption {display: block;position: absolute;bottom: 0;width: 100%;height: 100%;color: #fff;-webkit-transition: all .35s;-moz-transition: all .35s;transition: all .35s;}
.portfolio-box .portfolio-box-caption .portfolio-box-caption-content {position: absolute;top: 9%;left: 7%;width: 100%;}
.portfolio-box:hover .portfolio-box-caption {opacity: 1;}
</style>