<template>
  <div id="app">
    <h2 class="heading">Add</h2>
    <div class="row">
      <input v-model.number="num1" type="number">
      <span>+</span>
      <input v-model.number="num2" type="number">
      <span>=</span>
      <span>{{num1+num2}}</span>
    </div>
    <h2 class="heading">Subtact</h2>
    <div class="row">
      <input v-model.number="num3" type="number">
      <span>-</span>
      <input v-model.number="num4" type="number">
      <span>=</span>
      <span>{{num3-num4}}</span>
    </div>
    <h2 class="heading">Multiply</h2>
    <div class="row">
      <input v-model.number="num5" type="number">
      <span>*</span>
      <input v-model.number="num6" type="number">
      <span>=</span>
      <span>{{num5*num6}}</span>
    </div>
    <h2 class="heading">Divide</h2>
    <div class="row">
      <input v-model.number="num7" type="number">
      <span>/</span>
      <input v-model.number="num8" type="number">
      <span>=</span>
      <span>{{num7/num8}}</span>
    </div>
  </div>
</template>

<script>
export default {
  name: "app",
  data() {
    return {
      num1: 0,
      num2: 0,
      num3: 0,
      num4: 0,
      num5: 0,
      num6: 0,
      num7: 0,
      num8: 0
    };
  }
};
</script>

<style scoped>
#app {
  margin-left: 50%;
}
.row {
  /* display: flex; */
  /* justify-content: center; */
  font-family: "Work Sans", sans-serif;
}

input,
span {
  padding: 10px;
  font-size: 30px;
  font-family: "Work Sans", sans-serif;
}

input {
  width: 50px;
}

span {
  width: 20px;
}
/* .heading {
  margin-left: 50%;
} */
/* .second {
  font-size: 18px;
  p {
    margin-left: 20px;
  }
} */
</style>
