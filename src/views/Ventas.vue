<template>
  <div>
    <h1>Ventas de Juegos</h1>
    <section>
      <div class="input-group mb-3">
        <span class="input-group-text" id="formProductosConStok">
          Cantidad de productos con stock
        </span>
        <input
          type="text"
          class="form-control"
          v-model="getContador"
          aria-describedby="formProductosConStok"
          disabled
        />
      </div>
    </section>
    <section>
      <ListaJuegos :juegos="getListaDeJuegosContock" cantSell />
    </section>
  </div>
</template>

<script>
import { mapGetters } from "vuex";
import ListaJuegos from "@/components/ListaJuegos";

export default {
  name: "Ventas",
  components: { ListaJuegos },
  computed: {
    ...mapGetters(["getContador", "getListaDeJuegosContock"]),
  },
};
</script>

