<template>
  <div id="rete" v-show="visible" ref="rete"></div>
</template>

<script>
import init from "../node-editor";

export default {
  data() {
    return {
      visible: true
    };
  },
  methods: {
  },
  mounted() {
	init(this.$refs.rete);  
  }
};
</script>

<style>
#rete {
  width: 100%;
  height: 1000px;
}

.node .control input, .node .input-control input {
  width: 140px;
}

select, input {
  width: 100%;
  border-radius: 30px;
  background-color: white;
  padding: 2px 6px;
  border: 1px solid #999;
  font-size: 110%;
  width: 170px;
}
</style>
