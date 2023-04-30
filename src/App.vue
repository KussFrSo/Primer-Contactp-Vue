<template>
  <div></div>
  <ComputedComposition></ComputedComposition>
  <ComputedOptions></ComputedOptions>
  <WatchComposition></WatchComposition>
  <WatchOptions></WatchOptions>
  <PropsComposition first-name="Marc" last-name="Franch"></PropsComposition>
  <PropsOptions first-name="Marc" last-name="Franch"></PropsOptions>
  <ProvideInjectComposition></ProvideInjectComposition>
  <ProvideInjectOptions></ProvideInjectOptions>
  <RefsComposition></RefsComposition>
  <RefsOptions></RefsOptions>
</template>

<script>
import ComputedComposition from "./components/Computed/Computed-Composition.vue";
import ComputedOptions from "./components/Computed/Computed-Options.vue";
import WatchComposition from "./components/Watch/Watch-Composition.vue";
import WatchOptions from "./components/Watch/Watch-Options.vue";
import PropsComposition from "./components/Props/Props-Composition.vue";
import PropsOptions from "./components/Props/Props-Options.vue";
import ProvideInjectComposition from "./components/Provide-Inject/Provide-Inject-Composition.vue";
import ProvideInjectOptions from "./components/Provide-Inject/Provide-Inject-Options.vue";
import RefsComposition from "./components/Refs/Refs-Composition.vue";
import RefsOptions from "./components/Refs/Refs-Options.vue";

export default {
  components: {
    ComputedComposition,
    ComputedOptions,
    WatchComposition,
    WatchOptions,
    PropsComposition,
    PropsOptions,
    ProvideInjectComposition,
    ProvideInjectOptions,
    RefsComposition,
    RefsOptions,
  },
  provide: {
    appName: "Composition API vs Options API",
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
