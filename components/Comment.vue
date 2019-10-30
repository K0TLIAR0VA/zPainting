<template>
    <li>
        <p class="name">{{comment.name}}</p>
        <span class="date">{{comment.date.toLocaleString() }}</span>
        <p class="comment">{{comment.com}}</p>
    </li>
</template>

<script>
export default {
    props: ['comment']
}
</script>

<style scoped>
    li {border-bottom: 1px solid #e1e1e1;padding: 30px 0 50px;}
    .name {letter-spacing: 2.5px; color: #131313;}
    .comment {letter-spacing: 1px; line-height: 1em;}
    .date {margin-bottom: 8px;}
</style>