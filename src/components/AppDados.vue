<template>
  <div v-show="show" class=" bg-black bg-opacity-30 absolute top-0 left-0 w-full h-full flex justify-center z-50">
    <div class="bg-white self-center w-1/2 h-2/6 p-10 rounded-md drop-shadow-sm text-lg">
       <div class="container gap-6 max-w-md mx-auto rounded-full flex flex-col items-center bg-white h-12">
         <h1 class="text-3xl" >Digite seus dados</h1>
         <input class="container border border-black" type="text" placeholder="Digite seu nome">
         <input class="container border border-black" type="number" placeholder="Telefone">
         <input class="container border border-black" type="email" placeholder="E-mail">
       </div>
       <div class="flex flex-1 justify-end text-base mt-40 ">
        <AppButon class="text-green-500 hover:bg-green-500 hover:text-white">Salvar</AppButon>
        <AppButon class="text-red-500 hover:bg-red-500 hover:text-white" @click="close">Fechar</AppButon>
       </div>
    </div>
   
  </div>
  
</template>

<script setup>
import AppButon from "./AppButton.vue"
</script>

<script>
export default {
  data() {
    return{
      show: true
    }
  },
  methods: {
     open () {
        this.show = true
        console.log("chamou open");
      },
    close(){
      this.show = false
      console.log("chamou close");
    }
   
    
  },
};
</script>
