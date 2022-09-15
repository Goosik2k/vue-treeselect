<!-- eslint-disable -->

<template>
  <div>
    <treeselect :options="options" :multiple="multiple" />
    <label
      ><input type="checkbox" v-model="multiple" /> Multi-select mode</label
    >
  </div>
</template>

<script>
/* eslint-disable unicorn/no-abusive-eslint-disable */
/* eslint-disable */
import { generateOptions } from "../utils";

export default {
  data: () => ({
    options: generateOptions(1, 500),
  }),
};
</script>
