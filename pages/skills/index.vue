<template>
  <div>
    <h1>Skills (beta)</h1>

    <CheckList :items="responsibilities" header="Responsibilities" />

    <CheckList :items="skillsPreferred" header="Qualifications/Skills" />

    <CheckList
      :items="skillsOptional"
      header="Preferred Skills and Qualifications"
    />
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
import CheckList from '@/components/CheckList.vue'

export default Vue.extend({
  components: {
    CheckList
  },
  data() {
    return {
      responsibilities: [
        'Participate product/application development life cycle, including planning, analysis, design, implementation and maintenance, focus on UX/UI design both for PC and mobile.',
        'Implementing a front end for web applications with HTML/CSS/JavaScript according to demands from designers and planners',
        'Creating mockups and prototypes, verifying the output',
        'Proposing and designing UI with consideration of UX',
        'Write technical specifications based on conceptual design, business/technical requirements.',
        'Support short-term project like event or campaign to create campaign page or EDM.',
        'Researching and developing new web technologies',
        'Improving performance and maintaining products with high quality',
        'Implementing UI components and libraries',
        'System design and documentation'
      ],
      skillsPreferred: [
        'Expert knowledge of HTML/CSS/DOM/JavaScript',
        'Experience designing, developing and abstracting user interface elements and classes.',
        'Ability to work independently with HTML5, CSS3',
        'Experience developing PC/Smartphone web applications (3+years)',
        'Experience developing SPA (Single-page Applications)',
        'Fundamental knowledge of accessibility and usability',
        'Knowledge of CSS Preprocessors',
        'Experience prototyping tools like in Balsamiq, Adobe Illustrator, Photoshop, etc.'
      ],
      skillsOptional: [
        'Experience using tools for build and task runners (CI - continuous integration )',
        'Experience developing native iOS, Android applications',
        'Experience developing applications with server-side languages such as Java, Perl',
        'Familiarity with libraries such as Bootstrap, jQuery, Highcharts, etc.',
        'Contribution to OSS projects and communities',
        'Preferred knowledge of web performance technology.',
        'Experience in understanding large and complex code bases.',
        'Typically requires BSCS degree and 5+ years of directly related experience, or MSCS and 3+ years.'
      ]
    }
  }
})
</script>

<style scoped></style>
