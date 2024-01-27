<script setup lang="ts">
import { ref } from 'vue'
import Scroll from './Scroll.vue'

const langs = ref(["Ruby", "HTML5", "CSS3", "JavaScript", "TypeScript", "SQL", "PHP", "Visual Basic", "C#"]);
const devTools = ref(["git", "Visual Studio Code", "RubyMine", "Postman", "Chrome", "Sidekick", "Arc", "Edge", "Figma", "Firebase", "Supabase", "Adobe", "Docker", "Heroku"]);
const frameworks = ref(["Tailwind", "VueJS", "ReactJS", "Nuxt", "Ruby on Rails", "Bootstrap", "Postgresql", "Drupal", "Wordpress", "Umbraco"]);
const mgmt = ref(["Agile", "Scrum", "Jira", "GitHub", "GitLab", "Trello", "Monday"]);
</script>

<template>
  <div class="scroll-container">
    <Scroll timing="--time:40s" cssClass="scroll" :items=langs />
    <Scroll timing="--time:50s" cssClass="scroll-reverse" :items=devTools />
    <Scroll timing="--time:40s" cssClass="scroll" :items=frameworks />
    <Scroll timing="--time:50s" cssClass="scroll-reverse" :items=mgmt />
  </div>
</template>

<style scoped>
.scroll-container {
  display: flex;
  flex-direction: column;
  gap: 1rem;
}
</style>
