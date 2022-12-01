<template>
    <div>
        maincomptest
        <SearchComp />
       <!-- // <button @click="$emit(emitSearch, lorem)"></button> -->
    </div>
</template>

<script>
import SearchComp from "./SearchComp.vue";

export default {
  name: "MainComp",
  components: {
    SearchComp,
  },
};
</script>

<style>
</style>