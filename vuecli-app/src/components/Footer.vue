<template>
  <footer class="foot">
    <p>{{copyright}}{{title.name}}</p>
  </footer>
</template>

<script>
export default {
  name: "mr-header",
  props: {
    title: {
      type: Object,
      required: true
    }
  },
  data() {
    return {
      copyright: "Copyright 2019 Vue Footer"
    };
  }
};
</script>

<style scoped>
.foot {
  background: #222;
  padding: 10px;
}

p {
  color: lightgreen;
  text-align: center;
}
</style>