<template>
    <div>
        <Header></Header>
        <div class="not-found">
            <h2>404</h2>
            <p>Page not found</p>
            <a href="/" class="button">Go home</a>
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
.not-found {height: 100vh;background-image: url(../img/404.jpg);background-repeat: no-repeat;background-size: 100%;padding: 90px;}
h2 {font-size: 100px;font-weight: 400;letter-spacing: 1px;line-height: 1.2;color: #666;}
p {font-size: 50px;font-weight: 400;letter-spacing: 1px;line-height: 1.2;color: #666;}
.button {cursor: pointer;background-color: #575756;border-radius: 3px;width: 150px;color: #ffffff;padding: 15px;display: block;margin-top: 40px;text-transform: uppercase;text-align: center;font-size: 20px;}
</style>