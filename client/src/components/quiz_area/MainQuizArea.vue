<template>
    <div class="quiz-container">
        <div class="quiz-question">Answer to this question?</div>
        <div class="quiz-questions">questions</div>
        <div class="quiz-answers">answers</div>
        <div class="quiz-jokers">jokers</div>
        <div class="quiz-score">score</div>
        <div class="quiz-bid">bid</div>
    </div>
</template>

<script>
export default {
    
}
</script>

<style lang="scss" scoped>
    .quiz-container{
        display: grid;
        width: 100%;
        height: 100%;
        margin-top: 1rem;
        grid-template-columns: repeat(3, 1fr);
        grid-template-rows: repeat(4, minmax(6rem, auto));
        grid-template-areas: 
        "question question questions"
        "answers answers questions"
        "jokers jokers score"
        "... ... bid";
        grid-gap: .5rem;

        div{
            background-color: $primary-back-color;
            color: $primary-text-color
        }

        .quiz-question{
            grid-area: question;
            display: flex;
            justify-content: center;
            align-items: center;
        }
        .quiz-questions{
            grid-area: questions;
        }
        .quiz-answers{
            grid-area: answers;
        }
        .quiz-jokers{
            grid-area: jokers;
        }
        .quiz-score{
            grid-area: score;
        }
        .quiz-bid{
            grid-area: bid;
        }
    }

</style>