<script setup lang="ts">
import TheHeader from "./components/TheHeader.vue";
import SectionContact from "./components/SectionContact.vue";
import SectionExpertise from "./components/SectionExpertise.vue";
import SectionSkills from "./components/SectionSkills.vue";
import SectionEducation from "./components/SectionEducation.vue";
import SectionWork from "./components/SectionWork.vue";
import SectionSlotted from "./components/SectionSlotted.vue";
</script>
<template>
  <div class="layout">
    <TheHeader />
    <main class="main">
      <section class="main__start">
        <SectionContact />
        <SectionExpertise />
        <SectionSkills />
      </section>
      <section class="main__end">
        <SectionSlotted class="slotted-section">
          <template #title>Hello</template>
          <template #text>
            <p>
              Hi, I'm Brian and I solve puzzles for people. As both an
              enterprise-experienced developer and seasoned freelancer, my
              passion is helping people encounter an “ahhh” feeling while using
              software. However, an experience like this does not happen
              accidentally. It is through clear specs, accessible UX, clean
              code, and solid testing we create the most pleasing products
              possible. This is where I can add value to your team.
            </p>
          </template>
        </SectionSlotted>
        <SectionSlotted class="slotted-section">
          <template #title>My Story</template>
          <template #text>
            <p>
              While I am now a career-developer, for over ten years I was
              leading non-profit organizations. Through this decade I had the
              pleasure of leading scores of teams and developing hundreds of
              volunteers to impact their communities. In addition to leadership
              and management, I taught regularly, handled business meetings and
              budgets, and provided organizational leadership.
            </p>
            <p>
              While I was able to make a great impact on the communities I
              served, my family and I were beginning to burn out and knew it was
              time for a transition. For me, web development was the natural
              choice. A few years before leaving the non-profit world, I wrote
              my first Ruby on Rails app and sold it. After that moment, I was
              hooked. I started my freelancing business slinging Ruby on Rails,
              PHP, JavaScript, JQuery, and Cordova applications while working
              full-time.
            </p>
            <p>
              In 2020, after going full-time into the tech space, I was hired by
              the Ed Tech startup Campus Edu, as well as their parent company,
              Slingshot Edu, where I have been writing business-grade Vue.js
              applications.
            </p>
          </template>
        </SectionSlotted>
        <SectionSlotted class="slotted-section">
          <template #title>What You Can Expect</template>
          <template #text>
            <p>
              As a candidate, you can expect a high level of communication,
              leadership experience, and team member skills. On the technical
              side, I offer strong experience with modern frontend frameworks,
              storyboarding, UX design, ticketing systems, and testing. You will
              find through my references I am extremely high energy, teachable,
              focused, and of great integrity.
            </p>
          </template>
        </SectionSlotted>
        <SectionEducation />
        <SectionWork />
      </section>
    </main>
  </div>
</template>

<style lang="scss" scoped>
.main {
  display: grid;
  grid-template-columns: 1fr 2fr;

  section {
    padding: 0 0.75rem 0.75rem 0.75rem;
  }

  .slotted-section {
    p {
      text-indent: 2rem;

      &:not(:first-of-type):not(:last-of-type) {
        margin: 1rem 0;
      }
    }
  }

  &__start {
    background-color: var(--brian-accent);
  }
}
</style>
