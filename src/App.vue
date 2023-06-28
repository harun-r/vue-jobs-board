<template>
  <h3>{{name}} - {{ age }}</h3>
  <button @click="changeName('new name')">change name</button>
  <button @click="changeAge(15)">change Age</button>
</template>

<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({
  name: 'App',
  components: {},
  data() {
    return{
      name: 'Link',
      age: 25 as string | number
    }
  },
  methods:{
    changeName(name:string){
      this.name = name
      return name
    },
    changeAge(age: string | number){
      this.age = age
      return age
    }
  }
});
</script>

<style></style>
