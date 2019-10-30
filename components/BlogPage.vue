<template>
    <div>
        <Header></Header>
        <div class="blog">
            <div class="post" v-for="post in posts" :key="post.id">
                <span>{{post.date}}</span>
                <h2>{{post.title}}</h2>
                <span class="span">{{post.autor}}</span>
                <img :src="post.picture">
                <p>{{post.text}}</p>
                <a :href="post.href">Read More..</a>
            </div>
        </div>
        <Footer></Footer>
    </div>
</template>

<script>
import Header from './Header.vue';
import Footer from './Footer.vue';

export default {
    data: () => ({
        posts: [
            {
                date: 'June 8, 2016',
                title: 'Lorem ipsum dolor sit amet, consetetur sadipscing elitr',
                autor: 'ADMIN, LIFESTYLE',
                picture: require('../img/blog3.jpg'),
                text: 'Temporibus autem quibusdam et aut officiis debitis aut rerum necessitatibus saepe eveniet ut et voluptates repudiandae sint et molestiae non recusandae. Itaque earum rerum hic tenetur a sapiente delectus, ut aut reiciendis voluptatibus maiores alias consequatur aut perferendis doloribus asperiores repellat.…',
                href: '/post1'
            },
            {
                date: 'June 9, 2016',
                title: 'Eirmod tempor invidunt ut labore et dolore magna aliquyam erat',
                autor: 'ADMIN, LIFESTYLE',
                picture: require('../img/blog2.jpg'),
                text: 'Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque la udantium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi architecto beatae vitae dicta sunt explicabo. Nemo enim ipsam voluptatem quia.…',
                href: '/post2'
            },
            {
                date: 'June 10, 2016',
                title: 'Temporibus autem quibusdam et aut officiis debitis aut rerum necessitatibus saepe eveniet',
                autor: 'ADMIN, LIFESTYLE',
                picture: require('../img/blog4.jpg'),
                text: 'At vero eos et accusam et justo duo dolores et ea rebum. At vero eos et accusam et justo duo dolores et ea rebum. Consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. labore et dolore magna aliquyam erat, sed diam voluptua.…',
                href: '/post3'
            }
        ]}),

    components: {
        Header: Header,
        Footer: Footer,
    }
}
</script>

<style scoped>
.blog {max-width: 1200px;margin: 70px auto;}
.post {border-bottom: 1px solid #e1e1e1;padding: 30px 0 50px;}
p {margin: 40px 0;}
a {color: #888;}
.post:last-child {border-bottom: none;}
img {max-width: 1200px;margin-top: 40px;}
</style>