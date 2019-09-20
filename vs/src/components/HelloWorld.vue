<template>
  <div class="hello">
    <hr />
    <p>
      a ＜
      <!-- 複数class -->
      <!-- <span :class="{ big: isLarge, 'text-alert': hasError }">a</span> -->

      <!-- 配列構文、データバインディング -->
      <!-- <span :class="[largeClass, dangerClass]">a</span> -->

      <!-- データクラス、オブジェクト定義 -->
      <!-- <span :class="classObject">a</span> -->

      <!-- 三項演算子使用(その他の適用 ⇒ []を使用) -->
      <!-- <span :class="[isLarge ? largeClass : '', dangerClass]">a</span> -->

      <!-- インラインスタイルのデータバインド -->
      <!-- <span :style="{ color: color,  fontSize: fontSize + 'em' }">a</span> -->
      <!-- ケバブ使用の場合はこちら -->
      <!-- <span :style="{ color: color,  'font-size': fontSize + 'em' }">a</span> -->

      <!-- inline, object -->
      <span :style="styleObj">a</span>
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
      // 複数class
      // isLarge: true,
      // hasError: true

      // 配列構文、データバインディング
      // largeClass: "big",
      // dangerClass: "text-alert"

      // データクラス、オブジェクト定義
      // classObject: {
      //   big: true,
      //   "text-alert": true
      // }

      // 三項演算子使用
      // isLarge: true,
      // largeClass: "big",
      // dangerClass: "text-alert"

      // インラインスタイルのデータバインド
      // color: "red",
      // fontSize: 2

      // inline, object
      styleObj: {
        color: "red",
        fontSize: "5em"
      }
    };
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.big {
  font-size: 3rem;
}
.text-alert {
  color: #ff0000;
}

pre {
  text-align: left;
}
</style>
