<template>
    <div>
        <Header></Header>
        <article class="wrapper">
            <div class="header">
                <span class="date">June 8, 2019</span>
                <h1>Nulla eget mauris quis elit mollis ornare vitae ut odio augue vitae sollicitudin commodo</h1>
                <span class="name">ADMIN LIFESTYLE</span>
                <img src="../img/blog3.jpg" alt="">
                <div class="text">
                    <p>Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum exercitation ullamco laboris nisi ut aliquip.</p>
                    <p>Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum.</p>
                    <blockquote>
                        <p>Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet vultatup duista.</p>
                    </blockquote>
                    <p>Duis autem vel eum iriure dolor in hendrerit in vulputate velit esse molestie consequat, vel illum dolore eu feugiat nulla facilisis at vero eros et accumsan et iusto odio dignissim qui blandit praesent luptatum zzril.</p>
                    <h2>Heading 1</h2>
                    <p>Ut wisi enim ad minim veniam, quis nostrud exerci tation ullamcorper suscipit lobortis nisl ut aliquip ex ea commodo consequat. Duis autem vel eum iriure dolor in hendrerit in vulputate velit esse lorem ipsum dolor sit amet.</p>
                    <h2>Heading 2</h2>
                    <p>Duis autem vel eum iriure dolor in hendrerit in vulputate velit esse molestie consequat, vel illum dolore eu feugiat nulla facilisis. At vero eos et accusam et justo.</p>
                    <h2>Heading 3</h2>
                    <p>Consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum hendrerit in vulputate velit esse molestie.</p>
                    <p>Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum.</p>
                    <p><code>Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet.</code></p>
                    <p>Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet.</p>
                    <ol>
                        <li>Lorem ipsum</li>
                        <li>Sit amet vultatup nonumy</li>
                        <li>Duista sed diam</li>
                    </ol>
                    <p>Duis autem vel eum iriure dolor in hendrerit in vulputate velit esse molestie consequat, vel illum dolore eu feugiat nulla facilisis at vero eros et accumsan et iusto odio dignissim qui blandit praesent luptatum zzril delenit augue duis dolore te feugait nulla facilisi. Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut laoreet dolore magna aliquam erat volutpat.</p>
                    <p>Consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores.</p>
                </div>
            </div>
        </article>
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
.wrapper {background: #f6f6f6;padding: 30px 20px;}
span {text-align: center;display: block;}
.date {padding-bottom: 10px;}
.name {padding: 10px 0 40px;}
h1 {font-size: 58px;letter-spacing: 2px;font-weight: 300;text-transform: uppercase;line-height: 1.1;text-align: center;color: #3F3F3F;}
img {max-width: 1160px;}
.text {padding: 40px 120px;text-align: left;}
p {margin: 10px 0;}
blockquote {font-style: italic;border-left: 3px solid #1c7791;margin: 0 50px;color: #666;padding-left: 20px;}
h2 {letter-spacing: 1px;color: #3F3F3F;line-height: 1.2;font-size: 25px;}
code {color: #686868;font-size: 21px;font-family: monospace;}
ol {text-align: justify;margin: 10px 50px;list-style-type: circle;font-size: 21px;color: #3F3F3F;}
</style>