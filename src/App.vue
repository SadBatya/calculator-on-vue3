<template>
 <div class="max-w-full h-screen bg-blue-100 font-mono">
  <div class="w-4/5 mx-auto flex justify-center">
    <div class="bg-black rounded-xl p-2">
      <div>
        <div class="text-center text-white p-1">Calculator v1.0</div>
        <input v-model="value" type="number" class="w-full h-20 text-2xl p-2 bg-yellow-50 text-black rounded-t-md focus:outline-none focus:ring focus:border-blue-500">
      </div>
      <div class="text-white text-xl pt-2">
        <div>
          <button @click="clearValue" class="w-20 h-20 rounded-full bg-gray-500 m-0.5">AC</button>
          <button class="w-20 h-20 rounded-full bg-gray-500 m-0.5">+/-</button>
          <button class="w-20 h-20 rounded-full bg-gray-500 m-0.5">%</button>
          <button class="w-20 h-20 rounded-full bg-yellow-400 m-0.5">/</button>
        </div>
        <div>
          <button class="w-20 h-20 rounded-full bg-gray-300 m-0.5">1</button>
          <button class="w-20 h-20 rounded-full bg-gray-300 m-0.5">2</button>
          <button class="w-20 h-20 rounded-full bg-gray-300 m-0.5">3</button>
          <button class="w-20 h-20 rounded-full bg-yellow-400 m-0.5">X</button>
        </div>
        <div>
          <button class="w-20 h-20 rounded-full bg-gray-300 m-0.5">4</button>
          <button class="w-20 h-20 rounded-full bg-gray-300 m-0.5">5</button>
          <button class="w-20 h-20 rounded-full bg-gray-300 m-0.5">6</button>
          <button class="w-20 h-20 rounded-full bg-yellow-400 m-0.5">-</button>
        </div>
        <div>
          <button class="w-20 h-20 rounded-full bg-gray-300 m-0.5">7</button>
          <button class="w-20 h-20 rounded-full bg-gray-300 m-0.5">8</button>
          <button class="w-20 h-20 rounded-full bg-gray-300 m-0.5">9</button>
          <button class="w-20 h-20 rounded-full bg-yellow-400 m-0.5">+</button>
        </div>
        <div>
          <button class="w-20 h-20 rounded-full bg-gray-300 m-0.5">0</button>
          <button class="w-20 h-20 rounded-full bg-gray-300 m-0.5">.</button>
          <button class="w-40 h-20 rounded-full bg-yellow-400 m-0.5">=</button>
        </div>
      </div>
    </div>
  </div>
</div>
</template>

<script>
  export default{
    data(){
      return{
        value:''
      }
    },
    methods:{
      clearValue(){
        this.value = ''
      }
    }
  }
</script>

<style>

</style>
