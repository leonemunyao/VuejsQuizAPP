<script setup>
  import { defineProps } from 'vue';

  const {quiz} = defineProps(['quiz'])

</script>

<template>
    <div class="card">
        <img :src="quiz.img"
         alt="">
         <div class="card-text">
            <h2>{{ quiz.name }}</h2>
            <p>{{ quiz.questions.length }} Questions</p>
         </div>
    </div>
</template>

<style scoped>
        /* card styling */ 
        .card {
            width: 110px;
            overflow: hidden;
            border-radius: 2%;
            box-shadow: 1px 10px rgba(0, 0, 0, 0.1);
            margin-bottom: 35px;
            margin-right: 20px;
            cursor: pointer;
           } 
           .card img {
            width: 100%;
            height: 130px;
            margin: 0;
           }
           .card-text {
            padding: 0 5;
           }
           .card-text h2 {
            font-weight: bold;
           }    
</style>