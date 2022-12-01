<template>
  <div>
    <select name="" id="">
        <option v-for="(elem,index) in dischi" :key="index" value="index"
        @change="$emit('emitDischi' , elem)" >{{elem.genre}}</option>
    </select>
  </div>
</template>

<script>
import axios from "axios"

export default {
  name: "SearchComp",
data() {
    return {
    dischi : '',
    }
},
mounted () {
    this.recuperaDischi ()
    
},
methods : {
    recuperaDischi () {
        axios.get('https://flynn.boolean.careers/exercises/api/array/music')
        .then((response) => {
            this.dischi = response.data.response
            
        })
    }


},
computed : {

},
}
</script>

<style lang="scss" scoped>
</style>