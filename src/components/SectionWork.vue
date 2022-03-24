<script setup lang="ts">
import SectionTitle from "@/components/blocks/SectionTitle.vue";
import WorkGroup from "@/components/blocks/WorkGroup.vue";

const workData = [
  {
    position: "Frontend / Full-Stack Developer",
    company: "Slingshot Edu / Campus Edu",
    location: "USA ( Marion, IN )",
    date: "2020 - Present",
    description:
      "Since 2020 I have been developing enterprise-level Vue 2 and Vue 3 applications for the Ed Tech companies Slingshot Edu and Campus Edu. In this position, I am responsible for participating in spec meetings, spinning up Jira tickets, hashing out architecture patterns with the team, developing new features, enforcing AX standards, and writing tests. In addition to our modern stack, I was the sole Full-Stack Moodle ( PHP ) developer on the team.",
  },
  {
    position: "Full-Stack Developer",
    company: "Nerd Specs Creative",
    location: "USA ( Battle Creek, MI )",
    date: "2014 - Present",
    description:
      "In 2014, I began developing web applications with Ruby on Rails and launched my own company. As I work with clients, I have been able to touch several languages, frameworks, and stacks. I believe the past eight years of doing agency work has given me the unique ability to understand user stories and consider the positives and negatives when adopting the best tools.",
  },
  {
    position: "Lead Pastor",
    company: "New Journey Community Church",
    location: "USA ( Wabash, IN )",
    date: "2016 - 2020",
    description:
      "In 2016, the Scramlin family took our first lead pastoring position. New Journey Community Church was a six-year-old church plant seeking a leader with a balance between start-up charisma and long-range strategic planning. In only four years, I led the church in an increase of 20% attendance, growing the budget over 64%, and completed $250,000 in renovations. My heart for scalable, sustainable solutions led me to develop eight departments and heads, each overseeing ministry teams and leaders, who in turn oversee scores of volunteers. Most importantly, we have seen lives change. The hurting, addicted, de-churched, un-churched, disabled, and ashamed have found healing through our efforts. We give God the credit.",
  },
  {
    position: "Leadership, Discipleship, and Connections Pastor",
    company: "Spooner Wesleyan Church",
    location: "USA ( Spooner, WI )",
    date: "2013 - 2016",
    description:
      "In 2013, my wife and I took a big jump and moved to Northwest Wisconsin to undertake a re-envisioning position for a strong, traditional church of 400. I enjoyed the privilege of leading strategy and implementation teams for Discipleship, Connections, and Leadership, in addition to preaching on a rotation with our senior pastor. By inspiring, developing, and mobilizing the congregation and 85+ volunteers we witnessed a great deal of new fruit—especially in the outreach focus of this church!",
  },
];
</script>
<template>
  <section class="work">
    <SectionTitle title="Work Experience" />
    <div class="work__list">
      <WorkGroup
        v-for="work in workData"
        :key="work.company"
        :position="work.position"
        :company="work.company"
        :location="work.location"
        :date="work.date"
        :description="work.description"
      />
    </div>
  </section>
</template>

<style scoped lang="scss">
.work {
  &__list {
    display: grid;
    grap: 1rem;
  }
}
</style>
