<template>
  <p>question page 1</p>
  <p>{{ questions }}</p>

  <QuestionsList>
    <template v-slot="{ questions }">
      <ul>
        <li v-for="question in questions" :key="question">
          {{ question }}
        </li>
      </ul>
    </template>
  </QuestionsList>
</template>

<script>
import QuestionsList from "../components/QuestionsList.vue";

export default {
  setup() {},
  components: {
    QuestionsList,
  },
  data() {
    return {
      questions: "hello questions",
    };
  },
};
</script>

<style></style>
