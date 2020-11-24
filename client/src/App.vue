<template>
    <div class="main-container">
        <the-header></the-header>
        <main-quiz-area></main-quiz-area>
    </div>
</template>

<script>
import TheHeader from './components/layout/TheHeader.vue';
import MainQuizArea from './components/quiz_area/MainQuizArea.vue';

export default {
    components:{
        TheHeader,
        MainQuizArea
    }
}
</script>

<style lang="scss">
    .main-container{
        margin: 0 20%;
    }
</style>