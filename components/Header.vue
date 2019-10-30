<template>
    <header class="header">
        <div class="row1">
            <div class="social">
                <a href="#" class="after">Facebook</a>
                <a href="#" class="after">Instagram</a>
                <a href="#" class="after">Twitter</a>
                <a href="#" class="after">Google +</a>
                <a href="#">Pinterest</a>
            </div>
            <div class="top-search">
                <form id="form-container" action="">
                    <a class="search-submit-button" href="#"><i class="fa fa-search"></i></a>
                    <div id="searchtext"><input type="text" name="" placeholder="Search"></div>
                </form>
            </div>
        </div>
        <div class="row2">
            <img src="../img/logo.png" alt="">
        </div>
        <div class="row3">
            <nav>
                <a href="/">home</a>
                <a href="/about">about</a>
                <a href="/blog">blog</a>
                <a href="/contacts">contacts</a>
            </nav>
        </div>
    </header>
</template>

<style scoped>
.header {
    height: 350px;
    background: black;
}
.header .row1 {
    display: flex;
    max-width: 1200px;
    margin: 0 auto;
    padding: 20px;
    margin-bottom: 40px;
    justify-content: space-between;
}
.header .row1 .social {
    margin: auto 0;
}
.header .row1 .social a {
    color: #888888;
    letter-spacing: 1px;
}
.header .row1 .social .after::after {
    content: "-";
    padding: 0 10px;
}
.header .row1 .social a:hover{
    color: white;
}
#searchtext input {
    border: 1px solid #888;
    color: #fff;
    display: block;
    padding: 10px;
    width: 100%;
    box-sizing: border-box;
    font-size: 15px;
    margin: 0;
    background-color: transparent;
    height: 42px;
}
#form-container {
    max-width: 360px;
    text-align: center;
}
#searchtext {
    overflow: hidden;
}
a.search-submit-button {
    background: #fff;
    border-bottom: 1px solid #eeeeee;
    border-right: 1px solid #eeeeee;
    border-top: 1px solid #eeeeee;
    color: #131313;
    display: block;
    float: right;
    padding: 10px;
    font-size: 17px;
    text-align: center;
    width: 45px;
    box-sizing: border-box;
    height: 42px;
}
.header .row2 {
    width: 300px;
    margin: 0 auto;
}
.header .row2 img {
    width: 300px;
}
.header .row3 nav {
    display: flex;
    justify-content: center;
}
.header .row3 nav a {
    display: block;
    color: #ccc;
    padding: 15px 20px;
    text-transform: uppercase;
    font-size: 28px;
}
.header .row3 nav a:hover {
    background: white;
    color: black;
}
</style>>
