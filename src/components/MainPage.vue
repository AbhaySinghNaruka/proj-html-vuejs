<template>
  <main>
    <SectionOne />
    <SectionTwo />
    <SectionThree />
    <SectionFour />
    <SectionFive />
    <SectionSix />
    <FooterPage />
  </main>

</template>

<script>
import SectionOne from '@/components/SectionOne.vue';
import SectionTwo from '@/components/SectionTwo.vue';
import SectionThree from './SectionThree.vue';
import SectionFour from './SectionFour.vue';
import SectionFive from './SectionFive.vue';
import SectionSix from './SectionSix.vue';
import FooterPage from './FooterPage.vue';

export default {
  components: {
    SectionOne,
    SectionTwo,
    SectionThree,
    SectionFour,
    SectionFive,
    SectionSix,
    FooterPage,
  },
};
</script>

<style lang="scss" scoped>

</style>
