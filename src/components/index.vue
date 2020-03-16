<template>
  <div>
    <h3 style="text-align: center;">InputNumber 计数器</h3>
    <wmmInput v-model="value" :disabled="false" :step="2" @change="handleChange"></wmmInput>
  </div>
</template>

<script>
import wmmInput from "@/components/wmmInput";
export default {
  components:{
      wmmInput
  },
  data () {
    return {
     value:0
    }
  },
  methods:{
    handleChange(val) {
      console.log(val);
    },
  }
}
</script>

<style scoped>
h1, h2 {
  font-weight: normal;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
