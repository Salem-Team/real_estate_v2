<template>
  <!-- card 2 with props src -->
  <div class="m-2 h-[400px]">
    <div class="h-full card2-background shadow text-start">
      <div class="p-5">
        <div class="w-[200px]">
          <img
            class="w-full"
            :src="require(`../assets/media/${props.src}`)"
            alt="Card Image"
          />
        </div>
        <div>
          <h5 class="text-black text-xl mt-7">Budget Friendly</h5>
          <p class="text-sm mt-2">
            Distinctively re-engineer revolutionary meta-services and premium At
            vero eos et accusamus et iusto odio dignissimos ducimus qui
            blanditiis
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
// eslint-disable-next-line vue/no-setup-props-destructure
import { defineProps } from "vue";

const props = defineProps({
  src: {
    type: String,
    required: true,
  },
});
</script>

<style scoped>
/* Your styles */
</style>
