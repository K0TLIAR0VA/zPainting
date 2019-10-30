<template>
    <div>
        <Header></Header>

        <div class="wrapper">
            <h3>Contact form</h3>
            <form action="" method="" name="form1">
                <label for="" class="row">
                    <input type="text" name="name" placeholder="Enter name">
                    <input type="text" name="email" placeholder="Enter email">
                    <input type="text" name="subject" placeholder="Subject">
                </label>
                <label for="" class="row">
                    <textarea name="message" id="" cols="25" rows="4" placeholder="Message"></textarea>
                </label>
                <label for="" class="row">
                    <input type="submit" name="Submit" value="Submit" class="button">
                </label>
            </form>
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
.wrapper {background: #f6f6f6;padding: 70px;}
h3 {font-size: 57px;font-weight: 400;text-align: center;letter-spacing: 1px;line-height: 1.2;color: #666;}
form{padding: 20px 70px 0;}
.row {display: flex;justify-content: space-between;}
input, textarea{border: 1px solid #d1d1d1;color: #222;font-size: 16px;line-height: 1.2;margin-bottom: 23px;padding: 23px;}
.row input{width: 25%;height: 50px;}
.row textarea {height: 250px;width: 100%;}
.button {cursor: pointer;background-color: #575756;border-radius: 3px;width: 20%;color: #ffffff;padding: 15px;display: block;margin: 0 auto;margin-top: 50px;}
</style>