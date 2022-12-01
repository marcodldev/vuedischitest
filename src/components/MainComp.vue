<template>
    <div>
        maincomptest
        <SearchComp />
        <div @emitDischi="mostraDischi">
            {{elementoEmittato}}
        </div>
    </div>
</template>

<script>
import SearchComp from "./SearchComp.vue";

export default {
  name: "MainComp",
  components: {
    SearchComp,
  },
  data () {
    return {
        elementoEmittato : {}
    }
    
  },
  methods: {
    mostraDischi (elem) {
        console.log(elem);
      return this.elementoEmittato = elem
    }
},
mounted : {
      mostraDischi () {
        
      },
},
};
</script>

<style>
</style>