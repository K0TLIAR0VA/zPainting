<template>
    <div>
        <Header></Header>
        <div class="wrapper">
            <div class="img"><img src="../img/image19.jpg" alt=""></div>
            <div class="comment-wrap">
                <FormForComments @createTweet="addTweet"></FormForComments>
                <ol v-if="comments.length"><Comment v-for="comment in comments" :key="comment.id" v-bind:comment="comment"></Comment></ol>
            </div>
        </div>
        <Footer></Footer>
    </div>
</template>

<script>
import Header from './Header.vue';
import Footer from './Footer.vue';
import Comment from './Comment.vue';
import FormForComments from './FormForComments.vue';

export default {
    data: () => ({
        comments: [
            {
                name: 'Iryna',
                date: '21.08.2019, 20:30:42',
                com: 'Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua.'
            },
            {
                name: 'Vytalii',
                date: '18.09.2019, 15:35:37',
                com: 'Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua.'
            }

        ],
    }),

    methods: {
        addTweet(tweet) {
            console.log(tweet);
            this.comments.push(tweet);
        }
    },

    components: {
        Header, Footer, Comment, FormForComments,
    }
}
</script>

<style scoped>
.wrapper {display: flex;}
.comment-wrap {margin-left: 70px;padding: 70px;background: #f6f6f6;}
li {margin-bottom: 20px;}

</style>