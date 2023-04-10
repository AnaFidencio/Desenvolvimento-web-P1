<script setup>

</script>

<template>
  <form class="row g-3">
    <div class="container">
      <div class="row">
        <label for="staticEmail2" class="visually-hidden">Email</label>
        <input type="text" readonly class="form-control-plaintext" id="staticEmail2" placeholder="exemple@.com">
      </div>
      <div class="col-auto">
        <label for="inputPassword2" class="visually-hidden">Senha:</label>
        <input type="password" class="form-control" id="inputPassword2" placeholder="Password">
      </div>
      <div class="col-md-4">
        <label for="validationServer01" class="form-label">confirme a sua senha:</label>
        <input type="text" class="form-control is-valid" id="validationServer01" value="" required>
      </div>

      <div class="col-md-4">
        <label for="validationServer01" class="form-label">Primeiro nome:</label>
        <input type="text" class="form-control is-valid" id="validationServer01" value="" required placeholder="Ana">
      </div>
      <div class="col-md-4">
        <label for="validationServer02" class="form-label">Sobrenomes</label>
        <input type="text" class="form-control is-valid" id="validationServer02" value="" required placeholder="Silva">
      </div>
      <div class="col-md-4">
        <label for="validationServerUsername" class="form-label">escolha um nome de usuário</label>
        <div class="input-group has-validation">
          <span class="input-group-text" id="inputGroupPrepend3">@</span>
          <input type="text" class="form-control is-invalid" id="validationServerUsername"
            aria-describedby="inputGroupPrepend3 validationServerUsernameFeedback" required placeholder="exemple.12">
          <div id="validationServerUsernameFeedback" class="invalid-feedback">
            Por favor, escolha um nome de usuário.
          </div>
        </div>
      </div>
      <div class="col-md-3">
        <label for="validationServer04" class="form-label">Estado</label>
        <select class="form-select is-invalid" id="validationServer04" aria-describedby="validationServer04Feedback"
          required>
          <option selected disabled value="">selecionar</option>
          <option>(AC)Acre</option>
          <option>(AL)Alagoas</option>
          <option>(AP)Amapá</option>
          <option>(AM)Amazonas</option>
          <option>(BA)Bahia</option>
          <option>(CE)Ceará</option>
          <option>(DF)Distrito Federal</option>
          <option>(ES)Espírito Santo</option>
          <option>(GO)Goias</option>
          <option>(MA)Maranhão</option>
          <option>(MT)Mato Grosso</option>
          <option>(MS)Mato Grosso do Sul</option>
          <option>(MG)Minas Gerais</option>
          <option>(PA)Para</option>
          <option>(PB)Paraiba</option>
          <option>(PR)Paraná</option>
          <option>(PE)Pernambuco</option>
          <option>(PI)Piauí</option>
          <option>(RJ)Rio de Janeiro</option>
          <option>(RN)Rio Grande do Norte</option>
          <option>(RS)Rio Grande do Sul</option>
          <option>(RO)Rondônia</option>
          <option>(RR)Roraima</option>
          <option>(SC)Santa Catarina</option>
          <option>(SP)São Paulo</option>
          <option>(SE)Sergipe</option>
          <option>(TO)Tocantins</option>
        </select>
        <div id="validationServer04Feedback" class="invalid-feedback">
          Selecione um Estado válido.
        </div>
      </div>
      <div class="col-md-6">
        <label for="validationServer03" class="form-label">Cidade</label>
        <input type="text" class="form-control is-invalid" id="validationServer03"
          aria-describedby="validationServer03Feedback" required>
        <div id="validationServer03Feedback" class="invalid-feedback">
          Por favor, informe uma cidade válida.
        </div>
      </div>
       <div class="form-group">
    <label for="inputAddress">Endereço</label>
    <input type="text" class="form-control" id="inputAddress" placeholder="Rua dos Bobos, nº 0">
  </div>

      <div class="col-md-3">
        <label for="validationServer05" class="form-label">CPF</label>
        <input type="text" class="form-control is-invalid" id="validationServer05"
          aria-describedby="validationServer05Feedback" required>
        <div id="validationServer05Feedback" class="invalid-feedback">
          Informe um CPF válido.
        </div>
      </div>
      <div class="col-12">
        <div class="form-check">
          <input class="form-check-input is-invalid" type="checkbox" value="" id="invalidCheck3"
            aria-describedby="invalidCheck3Feedback" required>
          <label class="form-check-label" for="invalidCheck3">
            Concorde com os termos e condições
          </label>
          <div id="invalidCheck3Feedback" class="invalid-feedback">
            Você deve concordar antes de enviar.
          </div>
        </div>
      </div>
      <div class="col-12">
        <button class="btn btn-primary" type="submit">Enviar formulário</button>
      </div>
    </div>
  </form>
</template>

<style scoped></style>
