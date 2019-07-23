<template>
  <div class="py-12 tracking-wider">
    <div id="resume" class="flex flex-col md:resume shadow-2xl mx-auto bg-white sm:rounded-lg border-t-2 border-b-2 sm:border-2 border-gray-400">
      <div class="flex-grow">
        <resume-header />
        <div class="flex flex-wrap mx-10">
          <resume-experience />
          <div class="hidden sm:inline w-1/12"></div>
          <div class="order-first sm:order-none w-full sm:w-4/12">
            <resume-edu-skills />
          </div>
        </div>
        <resume-highlights />
      </div>
      <resume-footer />
    </div>
  </div>
</template>

<script>
import ResumeHeader from './ResumeHeader';
import ResumeExperience from './ResumeExperience';
import ResumeEduSkills from './ResumeEduSkills';
import ResumeHighlights from './ResumeHighlights';
import ResumeFooter from './ResumeFooter';

export default {
  components: { ResumeHeader, ResumeExperience, ResumeEduSkills, ResumeHighlights, ResumeFooter },
}
</script>

<style lang="sass">
@import url('https://fonts.googleapis.com/css?family=Monsterrat&display=swap')
#resume
  font-family: 'Monsterrat', sans-serif
</style>
