<template>
  <div>
    <h1>Total</h1>
    <section>
      <div class="input-group mb-3">
        <span class="input-group-text" id="formMontoTotalVentas">Monto Total Ventas</span>
        <input
          type="text"
          class="form-control"
          v-model="getTotalMonto"
          aria-describedby="formMontoTotalVentas"
          disabled
        />
      </div>
    </section>
    <section>
      <ListaVentas :ventas="ventas" />
    </section>
  </div>
</template>

<script>
import { mapGetters, mapState } from "vuex";
import ListaVentas from "@/components/ListaVentas";

export default {
  name: "Total",
  components: {
    ListaVentas,
  },
  computed: {
    ...mapState(["ventas"]),
    ...mapGetters(["getTotalMonto"]),
  },
};
</script>

<style></style>
