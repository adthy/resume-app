<template>
  <div class="tracking-wider">
    <div id="resume" class="flex flex-col resume mx-auto bg-white border-gray-400">
      <div class="flex-grow">
        <resume-header />
        <div class="flex flex-wrap mx-10">
          <resume-experience />
          <div class="inline w-1/12"></div>
          <div class="order-none w-4/12">
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

@page
  size: auto
  margin: 0mm
</style>
