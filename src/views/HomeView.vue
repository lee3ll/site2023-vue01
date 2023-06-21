<template>
  <main>
    <SliderSection attr="slider__wrap section gmarket5" />
    <IntroSection attr="intro__wrap section bg-blue gamrket5" />
    <!-- <MemberSection /> -->
    <PortSection attr="port__wrap gmarket5 section center bg-blue" />
    <YoutubeSection attr="youtube__wrap gmarket5 section" />
    <UnsplashSection attr="movie__wrap gmarket5 section" />
    <MovieSection attr="unsplash__wrap gmarket5 section bg-blue" />
  </main>
</template>

<script>
import SliderSection from "@/components/section/SliderSection.vue";
import IntroSection from "@/components/section/IntroSection.vue";
// import MemberSection from "@/components/section/MemberSection.vue";
import PortSection from "@/components/section/PortSection.vue";
import YoutubeSection from "@/components/section/YoutubeSection.vue";
import UnsplashSection from "@/components/section/UnsplashSection.vue";
import MovieSection from "@/components/section/MovieSection.vue";

export default {
  components: {
    SliderSection,
    IntroSection,
    // MemberSection,
    PortSection,
    YoutubeSection,
    UnsplashSection,
    MovieSection,
  },
};
</script>
