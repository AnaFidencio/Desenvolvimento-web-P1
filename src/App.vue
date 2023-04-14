<script setup>
import { ref } from 'vue'
const email = ref('')
const senha = ref('')
const confirmaSenha = ref('')
const nome = ref('')
const nascimento = ref('')
const bairro = ref('')
const numero = ref('')
const complemento = ref('')
const cidade = ref('')
const estado = ref('')
const hobbies = ref('')
const liguagensProg = ref('')
const biografia = ref('')
const enviar = ref(false)
const erro = ref('')

function confirmacao() {
  if (senha.value === confirmaSenha.value) {
    erro.value = "";
    return true;
  } else {
    erro.value = "A senha não confere!"
    return false
  }
}
</script>

<template>
  <div>
    <form class="formulario" @submit.prevent="enviar = confirmacao()">
      <h1>Login</h1>
      <div class="nome">
        <h4>Informe seu nome</h4>
        <input type="text" v-model="nome" v-on:keypress="enviar = false" placeholder="Eduardo " required>
      </div>
      <div class="email">
        <h4>Informe seu email</h4>
        <input type="email" v-model="email" v-on:keypress="enviar = false" placeholder="example@gmail" required>
      </div>
      <div class="senha">
        <h4>Crie uma senha</h4>
        <input type="password" v-model="senha" v-on:keypress="enviar = false" placeholder="senha" required>
      </div>
      <div class="confirmaSenha">
        <h4>Confirme sua senha</h4>
        <input type="password" v-model="confirmaSenha" v-on:keypress="enviar = false" placeholder="confirma senha"
          required>
      </div>
      <div class="nascimento">
        <h4>Informe sua data de nascimento</h4>
        <input type="date" v-model="nascimento" v-on:keypress="enviar = false" required>
      </div>
      <div class="bairro">
        <h4>Informe seu bairro</h4>
        <input type="text" v-model="bairro" v-on:keypress="enviar = false" placeholder="bairro" required>
      </div>
      <div class="numero">
        <h4>Informe o número da casa</h4>
        <input type="number" v-model="numero" v-on:keypress="enviar = false" placeholder="°n" required>
      </div>
      <div class="complemento">
        <h4>Adicione um complemento (opcional)</h4>
        <input type="text" v-model="complemento" placeholder="complemento" required>
      </div>
      <div class="cidade">
        <h4>Informe a sua cidade</h4>
        <input type="text" v-model="cidade" v-on:keypress="enviar = false" placeholder="cidade" required>
      </div>
      <div class="estado">
        <h4>Informe o seu estado</h4>
        <select v-model="estado" v-on:keypress="enviar = false" required>
          <option value="AC">Acre</option>
          <option value="AL">Alagoas</option>
          <option value="AP">Amapá</option>
          <option value="AM">Amazonas</option>
          <option value="BA">Bahia</option>
          <option value="CE">Ceará</option>
          <option value="ES">Espírito Santo</option>
          <option value="GO">Goiás</option>
          <option value="MA">Maranhão</option>
          <option value="MT">Mato Grosso</option>
          <option value="MS">Mato Grosso do Sul</option>
          <option value="MG">Minas Gerais</option>
          <option value="PA">Pará</option>
          <option value="PB">Paraíba</option>
          <option value="PR">Paraná</option>
          <option value="PE">Pernambuco</option>
          <option value="PI">Piauí</option>
          <option value="RJ">Rio de Janeiro</option>
          <option value="RN">Rio Grande do Norte</option>
          <option value="RS">Rio Grande do Sul</option>
          <option value="RO">Rondônia</option>
          <option value="RR">Roraima</option>
          <option value="SC">Santa Catarina</option>
          <option value="SP">São Paulo</option>
          <option value="SE">Sergipe</option>
          <option value="TO">Tocantins</option>
        </select>
      </div>
      <div class="hobbies">
        <h4>Informe seus Hobbies</h4>
        <textarea name="Hobbies" v-model="hobbies" cols="30" rows="5" v-on:keypress="enviar = false"></textarea>
      </div>
      <div class="linguagensProg">
        <h4>Informe as linguagens de programação</h4>
        <textarea name="LiguagensdeProg" v-model="liguagensProg" cols="30" rows="5"
          v-on:keypress="enviar = false"></textarea>
      </div>
      <div class="biografia">
        <h4>Escreva uma biografia</h4>
        <textarea name="Hobbies" v-model="biografia" cols="30" rows="5" v-on:keypress="enviar = false"></textarea>
      </div>
      <button type="submit">Enviar</button>
    </form>
    <p>{{ erro }}</p>
  </div>

  <div v-if="enviar" class="cadastro">
    <h1>Cadastro de perfil</h1>
    <p>Nome: {{ nome }}</p>
    <div class="email-atual">
      <p>Email: {{ email }}</p>
    </div>
    <div class="senha-atual">
      <p>Senha: {{ senha }}</p>
    </div>
    <div class="nascimento-atualizado">
      <p>Data de nascimento: {{ nascimento }}</p>
    </div>
    <div class="bairro-atual">
      <p>Bairro: {{ bairro }}</p>
    </div>
    <div class="numero-atual">
      <p>Número da casa: {{ numero }}</p>
    </div>
    <div class="complemento-atual">
      <p>Complemento: {{ complemento }}</p>
    </div>
    <div class="cidade-atual">
      <p>Cidade: {{ cidade }}</p>
    </div>
    <div class="estado-atual">
      <p>estado: {{ estado }}</p>
    </div>
    <div class="hobbies">
      <p>Hobbies: {{ hobbies }}</p>
    </div>
    <div class="linguagens">
      <p>Linguagens de programação: {{ liguagensProg }}</p>
    </div>
    <div class="bio">
      <p>Biografia: {{ biografia }}</p>
    </div>
  </div>
</template>

<style scoped>
.formulario {
  background-color: cadetblue;
  border-radius: 30px;
  border-style: solid;
  padding: 10px;
}
</style>
