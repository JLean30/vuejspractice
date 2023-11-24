<template>
<div class="post-card">
    <h3>Titulo</h3>
    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Consequuntur, dolorum accusantium. Accusamus suscipit non cupiditate libero minima nemo provident aut quasi soluta in repudiandae, ut doloremque, quos laborum animi fugit!</p>
    <PostButton/>
</div>
</template>

<script lang="ts" setup>
import PostButton from './PostButton.vue';
</script>

<style scoped>
.post-card{
    border-radius: 15px;
    padding: 10px;
    margin: 5px;
    border: 1px solid #ccc;
}
</style>