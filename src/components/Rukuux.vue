<template>
  <v-container>
    <v-row class="text-center">
      <v-col cols="12">
        <v-img
          :src="require('../assets/logo.svg')"
          class="my-3"
          contain
          height="200"
        />
      </v-col>

      <v-col class="mb-4">
        <h1 class="display-2 font-weight-bold mb-3">
          Ütz iwäch pa qasamaj Atitya'
        </h1>

        <p class="subheading font-weight-regular">
          Tajin niqajunumaj etamab'äl chuqa' ruxe'el tzij
          <br>chirij ri choy Atitlan chuqa'.
          <a
            href="https://github.com/marcoramirez21/Yikbalruxetzijnaoj"
            target="_blank"
          >Tatz'u qasamaj wawe.</a>
        </p>
      </v-col>

      <v-col
        class="mb-5"
        cols="12"
      >
        <h2 class="headline font-weight-bold mb-3">
          ¿Achike chïk?
        </h2>

        <p class="subheading font-weight-regular">
          Xtiqajunumaj ri setul wawe.
        </p>

      </v-col>
    </v-row>
  </v-container>
</template>

<script>
  export default {
    name: 'Rukuux',

    data: () => ({
    }),
  }
</script>
