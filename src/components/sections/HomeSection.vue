<script setup lang="ts">
import Section from '@/components/Section.vue';
import IconLink from '@/components/IconLink.vue'
import EmailIcon from '@/components/icons/EmailIcon.vue';
import GitHubIcon from '@/components/icons/GitHubIcon.vue';
import LinkedInIcon from '@/components/icons/LinkedInIcon.vue';
import ResumeIcon from '@/components/icons/ResumeIcon.vue';
</script>

<template>
  <Section>
    <template #title>Aaron Lam</template>
    <ul>
      <li>
        <IconLink url="https://github.com/aaronlam1004">
          <GitHubIcon/>
        </IconLink>
      </li>
      <li>
        <IconLink url="https://www.linkedin.com/in/aaron-t-lam/">
          <LinkedInIcon/>
        </IconLink>
      </li>
      <li>
        <IconLink url="mailto:aaronlam1004@gmail.com">
          <EmailIcon/>
        </IconLink>
      </li>
      <li>
        <IconLink url="Aaron Lam's Resume.pdf">
          <ResumeIcon/>
        </IconLink>
      </li>
    </ul>
  </Section>
</template>

<style scoped>
ul {
  margin: 0;
  padding: 0;
  width: 100%;

  display: flex;
  flex-direction: row;
  justify-content: center;
}

ul li {
  padding-left: 0.5em;
  padding-right: 0.5em;
  list-style-type: none;
}

svg {
  margin: 0;
  position: relative;
  display: block;
  width: 2.25em;
  height: 2.25em;
  padding: 0.5em 0.5em;

}
</style>
