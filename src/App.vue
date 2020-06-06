<template>
  <div>
    <input type="text" v-model.number="inputField" />
    <div
      v-for="n in 10"
      :key="n"
    >Число {{n}} умноженное на число {{inputField}} = {{n * inputField}}</div>
  </div>
</template>

<script>
export default {
  name: "App",
  data: () => ({
    inputField: 0
  })
};
</script>
