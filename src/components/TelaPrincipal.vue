<template>
  <div id="tela">
    <h1>Ola Mundo</h1>
    <input v-model="nota" type="text" id="texto-nota" />
    <h1>{{ res }}</h1>
    <v-btn @click="alerta()" flat slot="Ativar" id="button" class="success"
      >Ativar</v-btn
    >

    <v-alert v-show="mostrar" shaped prominent type="error">
        Digite apenas notas
    </v-alert>
    <v-btn href="TelaPrincipal" @click="tentarNovamente" v-show="buttonOff" flat slot="Ativar" id="button" class="success"
      >Tentar novamente</v-btn
    >   

       <v-alert
      shaped
      prominent
      type="error"
    >
      I'm a shaped alert with a dense prominent option that Praesent blandit laoreet nibh. Praesent nonummy mi in odio. Phasellus tempus. Mauris turpis nunc, blandit et, volutpat molestie, porta ut, ligula. Duis leo.
    </v-alert>


  </div>
</template>


<script>
export default {
  name: "TelaPrincipal",
  data() {
    return {
      buttonOff:false,  
      mostrar: false,
      nota: "",
      res: this.nota,
    };
  },
  methods: {
    alerta() {
      if (this.nota == "C") {
        this.res = this.nota;
      } else {
        this.mostrar = true;
        this.buttonOff=!this.buttonOff
        
      }

      // this.mostrar = !this.mostrar
    },
    // tentarNovamente(){
    //     this.mostrar = false
    //     this.res = ""
    //     this.nota=""
    //     this.buttonOff=false
        
    // }

  },
};
</script>


<style>
</style>