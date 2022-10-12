

<template>
    <div class="tweet">
        <!-- <ProfileImage :image="user.image" /> -->
        <ProfileImage :image="tweet.user.image" />
        

        <!-- tweet.user.image -->
        <div class="body">
            <div class="top">
                    <User :userData="tweet.user" />
                    <TimeStamp :time="tweet.timestamp"/>
            </div>

            <Message :message="tweet.message"/>

            <Actions />
        </div>

        <i class="fas fa-ellipsis-h"></i>
    </div>
</template>
<script setup>


import ProfileImage from "./ProfileImage.vue"
import User from "./User.vue"
import TimeStamp from "./TimeStamp.vue"
import Message from "./Message.vue"
import Actions from "./Actions.vue"



const props = defineProps(['tweet'])


</script>
<style scoped>
a {
    color: #42b983;
}
</style>