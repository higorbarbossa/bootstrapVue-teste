<template>
  <div class="container">
    <div class="col-md-6">
      <b-form inline >
        <b-form-group  id="input-group-1" label="Numero de Identificação:" label-for="input-1">
          <b-form-input
            id="input-1"
            type="text"
            required
            placeholder="Numero de identificação do Ato"
          ></b-form-input>
        </b-form-group>
        <b-form-group id="input-group-3" label="Food:" label-for="input-2">
          <b-form-input
            id="input-2"
            type="text"
            required
            placeholder="Numero de identificação do Ato"
          ></b-form-input>
          <b-form-select id="input-2" :options="foods" required></b-form-select>
        </b-form-group>
        <div class="row">.</div>
      </b-form>
      <b-alert show>Default Alert</b-alert>

      <b-alert variant="success" show>Success Alert</b-alert>
    </div>
    <div class="col-md-6">
      <div class="row">....</div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      foods: [
        { text: "Select One", value: null },
        "Carrots",
        "Beans",
        "Tomatoes",
        "Corn"
      ]
    };
  },
  methods: {}
};
</script>