<template>
  <div>
    <input type="textarea" v-model.number="bilangan1" placeholder="Masukkan bilangan 1 ">
    <input type="textarea" v-model.number="bilangan2" placeholder="Masukkan bilangan 2 ">
    <button @click="hitung">HITUNG</button>
    <input type="number" :value="hasil" disabled>
  </div>
</template>

<script>
export default {
  data() {
    return {
      bilangan1: ' ',
      bilangan2: ' ',
      hasil: 0
    }
  },
  methods: {
    hitung() {
      this.hasil = this.bilangan1 + this.bilangan2;
    }
  }
}
</script>
