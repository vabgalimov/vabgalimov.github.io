<script setup>
import { socials } from "./lib/socials";
</script>

<template>
  <center>
    <img src="./assets/avatar.png" alt="avatar" class="avatar">
    <a href="https://mynickname.com/id1527041" id="nickname">
      <h3>vabgalimov</h3>
    </a>
    <div>
      <a v-for="social in socials" :href="social.url">
        <img :src="social.logo" :alt="social.name" class="icon">
      </a>
    </div>
  </center>
  <p><b>Hi there!</b></p>
  <p>I'm vabgalimov</p>
</template>

<style scoped>
  a {
    color: black;
    text-decoration: none;
  }
  .avatar {
    height: 100px;
    width: 100px;
  }
  .icon {
    height: 25px;
    width: 25px;
    margin-left: 5px;
    margin-right: 5px;
  }
</style>
