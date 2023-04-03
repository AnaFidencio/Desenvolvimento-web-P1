
<script setup>
import { ref } from 'vue'

const nome = ref('kkkkk')
</script>

<template>
  <form>
    <div class="mb-3">
      <label for="exampleInputEmail1" class="form-label">Email address</label>
      <input type="email" class="form-control" id="exampleInputEmail1" aria-describedby="emailHelp">
    </div>
    <div class="mb-3">
      <label for="exampleInputPassword1" class="form-label">Password</label>
      <input type="password" class="form-control" id="exampleInputPassword1">
      <div class="col-md-6">
    <label for="validationServer03" class="form-label">City</label>
    <input type="text" class="form-control is-invalid" id="validationServer03" aria-describedby="validationServer03Feedback" required>
    <div id="validationServer03Feedback" class="invalid-feedback">
      Please provide a valid city.
    </div>
  </div>
    </div>
  
    <select class="form-select" aria-label="Default select example">
    <option selected>Selecione o Estado</option>
    <option value="1">One</option>
    <option value="2">Two</option>
    <option value="3">Three</option>
    <option value="4">One</option>
    <option value="5">One</option>
    <option value="6">One</option>
    <option value="7">One</option>
    <option value="8">One</option>
    <option value="9">One</option>
    <option value="10">One</option>
    <option value="11">One</option>
    <option value="12">One</option>
    <option value="13">One</option>
    <option value="14">One</option>
    <option value="15">One</option>
    <option value="16">One</option>
    <option value="17">One</option>
    <option value="18">One</option>
    <option value="19">One</option>
    <option value="20">One</option>
    <option value="21">One</option>
    <option value="22">One</option>
    <option value="23">One</option>
    <option value="24">One</option>
    <option value="25">One</option>
    <option value="26">One</option>
    <option value="27">One</option>
  </select>
  <button type="submit" class="btn btn-primary">Submit</button>
  </form>
  
</template>

<style scoped></style>
