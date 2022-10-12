<template>
    <div class="tweet">
        <ProfileImage :image="tweet.user.image" />
        <!-- <img :src="tweet[0].user.image" class="profile" alt="profile" /> -->
        <div class="body">
            <div class="top">
                <User :userData="tweet.user" />
                <!-- <span class="name">{{tweet[0].user.name}}</span> -->
                <!-- <span class="handle">{{tweet[0].user.handle}}</span> -->
                <Timestamp :time="tweet.timestamp" />
            </div>

            <Message :message="tweet.message" />

            <!-- <p class="message">{{tweet[0].user.message}} </p>-->

            <Actions />
            
        </div>

        <i class="fas fa-ellipsis-h"></i>
    </div>
</template>

<script setup>
import ProfileImage from './ProfileImage.vue';
import User from './User.vue';
import Timestamp from './Timestamp.vue';
import Message from './Message.vue';
import Actions from './Actions.vue';

const props = defineProps(["tweet"]);
</script>

<style scoped>
a {
    color: #42b983;
}
</style>