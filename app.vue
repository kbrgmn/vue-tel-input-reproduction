<template>
  <div>
      <VueTelInput v-model="phone"/>
  </div>
</template>

<script lang="ts" setup>
import {VueTelInput} from 'vue-tel-input';
import 'vue-tel-input/vue-tel-input.css';

const phone = ref("")
</script>
