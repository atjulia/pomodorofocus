<template>
  <div class="flex item-center">
    <img src="https://github.com/atjulia.png" alt="Júlia Karolina" class="mr-6 w-20 h-20 rounded-full">
    <div class="flex flex-col w-full">
      <strong class="text-title text-2xl">Júlia Karolina</strong>
      <p class="flex flex-center">
        <img src="icons/level.svg" alt="level" class="mr-2">
        <span class="text-base">Level {{ level }}</span>
      </p>
    </div>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
import { mapState } from 'vuex' 

export default Vue.extend({
  computed: mapState('challenges', ['level'])
})
</script>