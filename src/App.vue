<template>
  <div
    class="bg-gray-300 inset-0 absolute flex flex-column items-center justify-center"
  >
    <check-box fieldId="volume" v-model:checked="volumeOn" label="Volume On" />
  </div>
</template>

<script>
import Checkbox from "./components/checkbox.vue";
import { ref } from "vue";
export default {
  name: "App",
  setup() {
    const volumeOn = ref(true);
    return {
      volumeOn,
    };
  },
  components: {
    "check-box": Checkbox,
  },
};
</script>

<style>
</style>
