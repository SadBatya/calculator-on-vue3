<template>
 <div class="max-w-full h-screen bg-blue-100 font-mono">
  <div class="w-4/5 mx-auto flex justify-center">
    <div class="bg-black rounded-xl p-2">
      <div>
        <div class="text-center text-white p-1">Calculator v1.0</div>
        <form class="flex h-20 text-2xl p-2 bg-yellow-50 text-black rounded-t-md focus:outline-none focus:ring focus:border-blue-500">
          <input v-model="value" type="text" class="bg-yellow-50 focus:outline-none">
          <button @click.prevent="this.value = value.slice(0, -1)">
            <img src="./assets/backspace.png" alt="backspace">
          </button>
        </form>
      </div>
      <div class="text-white text-xl pt-2">
        <div>
          <button @click="this.value = ''" class="w-20 h-20 rounded-full bg-gray-500 m-1.5">AC</button>
          <button @click="this.value += '+'" class="w-20 h-20 rounded-full bg-gray-500 m-1.5">+/-</button>
          <button @click="this.value += '%'" class="w-20 h-20 rounded-full bg-gray-500 m-1.5">%</button>
          <button @click="this.value += '/'" class="w-20 h-20 rounded-full bg-yellow-400 m-1.5">/</button>
        </div>
        <div>
          <button @click="this.value += '1'" class="w-20 h-20 rounded-full bg-gray-300 m-1.5">1</button>
          <button @click="this.value += '2'" class="w-20 h-20 rounded-full bg-gray-300 m-1.5">2</button>
          <button @click="this.value += '3'" class="w-20 h-20 rounded-full bg-gray-300 m-1.5">3</button>
          <button @click="this.value += '*'" class="w-20 h-20 rounded-full bg-yellow-400 m-1.5">X</button>
        </div>
        <div>
          <button @click="this.value += '4'" class="w-20 h-20 rounded-full bg-gray-300 m-1.5">4</button>
          <button @click="this.value += '5'" class="w-20 h-20 rounded-full bg-gray-300 m-1.5">5</button>
          <button @click="this.value += '6'" class="w-20 h-20 rounded-full bg-gray-300 m-1.5">6</button>
          <button @click="this.value += '-'" class="w-20 h-20 rounded-full bg-yellow-400 m-1.5">-</button>
        </div>
        <div>
          <button @click="this.value += '7'" class="w-20 h-20 rounded-full bg-gray-300 m-1.5">7</button>
          <button @click="this.value += '8'" class="w-20 h-20 rounded-full bg-gray-300 m-1.5">8</button>
          <button @click="this.value += '9'" class="w-20 h-20 rounded-full bg-gray-300 m-1.5">9</button>
          <button @click="this.value += '+'" class="w-20 h-20 rounded-full bg-yellow-400 m-1.5">+</button>
        </div>
        <div>
          <button @click="this.value += '0'" class="w-20 h-20 rounded-full bg-gray-300 m-1.5">0</button>
          <button @click="this.value += '.'" class="w-20 h-20 rounded-full bg-gray-300 m-1.5">.</button>
          <button @click="this.value += '='" class="w-40 h-20 rounded-full bg-yellow-400 m-1.5">=</button>
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
      
    }
  }
</script>

<style>

</style>
