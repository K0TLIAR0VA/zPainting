<template>
    <div>
        <Header></Header>
			<div class="wrapper">
				<a v-for="element in elements" v-bind:href="element.href" :key="element.id" >
					<img v-bind:src="element.src">
				</a>
			</div>
        <Footer></Footer>
    </div>
</template>

<script>
import Header from './Header.vue';
import Footer from './Footer.vue';

export default {
	data: () => ({
		elements: [
			{href: '/picture1', src: require('../img/image19.jpg')},
			{href: '/picture2', src: require('../img/image22.jpg')},
			{href: '/picture3', src: require('../img/image26.jpg')},
			{href: '/picture4', src: require('../img/image20.jpg')},
			{href: '/picture5', src: require('../img/image23.jpg')},
			{href: '/picture6', src: require('../img/image27.jpg')},
			{href: '/picture7', src: require('../img/image21.jpg')},
			{href: '/picture8', src: require('../img/image24.jpg')},
			{href: '/picture9', src: require('../img/image28.jpg')},
			{href: '/picture10', src: require('../img/image25.jpg')},
		],
	}),

    components: {
        Header: Header,
        Footer: Footer,
    }
}
</script>

<style scoped>
.wrapper {padding-bottom: 2460px;}
img {width: 100%;height: auto;position: absolute;overflow: hidden;}
a {position: relative;width: 390px;display: block;}
a:nth-child(2) {right: -405px;}
a:nth-child(3) {right: -810px;}
a:nth-child(4) {top: 758px;}
a:nth-child(5) {right: -405px; top: 622px;}
a:nth-child(6) {right: -810px; top: 553px;}
a:nth-child(7) {top: 1260px;}
a:nth-child(8) {right: -405px; top: 1134px;}
a:nth-child(9) {right: -810px; top: 1547px;}
a:nth-child(10) {right: -405px; top: 1974px;}
img:hover{border: solid 2px #131313;}
</style>