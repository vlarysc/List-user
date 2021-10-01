<template>
  <AppDados></AppDados>
  <div>
    <h1 class="">List User</h1>
    <div>
      <button class="border border-black p-2" @click="open">Novo Registro</button>
    </div>
    
    <thead class="flex ">
      <th class="px-3">Nome</th>
      <th class="px-3">Telefone</th>
      <th class="px-3">Email</th>
      <th class="px-3">Ações</th>
    </thead>

    <tbody>
      <tr> 
        <td></td>
      </tr>
    </tbody>
  </div>
</template>

<script setup>
import AppDados from "./components/AppDados.vue"
</script>

<script>
export default {
  data(){
    return {
          
    }
 },
 methods: {
   
 },
}
</script>