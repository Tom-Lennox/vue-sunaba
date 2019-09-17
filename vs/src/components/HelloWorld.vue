<template>
  <div class="hello">
    <hr />
    <p>
      a ＜
      <span :class="{ big: isLarge }">a</span>
    </p>
    <pre>{{$data}}</pre>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  data() {
    return {
      msg: "■",
      isLarge: true
    };
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1,
h2 {
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
