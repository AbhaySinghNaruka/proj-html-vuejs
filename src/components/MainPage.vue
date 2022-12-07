<template>
  <main>
    <SectionOne />
    <SectionTwo />
  </main>

</template>

<script>
import SectionOne from '@/components/SectionOne.vue';
import SectionTwo from '@/components/SectionTwo.vue';

export default {
  components: {
    SectionOne,
    SectionTwo,
  },
};
</script>

<style lang="scss" scoped>

main {
  height: 4500px;

}

</style>
