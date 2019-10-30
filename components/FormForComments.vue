<template>
    <form @submit="submit" class="form">
        <input type="text" v-model="userName" placeholder="Your name" class="input-name">
        <textarea type="text" cols="30" rows="10" v-model="userComment" placeholder="Your message"></textarea>
        <input type="submit" value="Submit" class="submit">
    </form>
</template>

<script>
export default {
    data: () => ({
        userName: '',
        userComment: '',
    }),

    methods: {
        submit(event) {
            event.preventDefault();
            const newTweet = { name: this.userName, com:this.userComment, date: new Date() };
            this.$emit('createTweet', newTweet)
            this.userName = '';
            this.userComment = '';
    }
}}
</script>

<style scoped>
input, textarea {display: block;margin-bottom: 5px;}
.input-name, textarea {width: 500px;border: 1px solid #d1d1d1;color: #222;font-size: 16px;line-height: 1.2;margin-bottom: 23px;padding: 23px;}
.input-name {height: 32px;}
.submit {cursor: pointer;background-color: #575756;border-radius: 3px;width: 20%;color: #ffffff;padding: 15px;display: block;margin-top: 20px;}
</style>