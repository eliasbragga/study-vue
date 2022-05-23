<template>
  <div id="app">
 
    <TelaPrincipal/>
  </div>
    
   
 
</template>

<script>
import TelaPrincipal from './components/TelaPrincipal.vue';



export default {
  name: 'App',

  components: {
    TelaPrincipal
},

  data(){
    return{     

    }
    
  },
  methods:{
    
  }
};
</script>

<style>
#tela{
  color: rgb(31, 31, 31);
}


.theme--light.v-btn.v-btn--has-bg {
   
}

.v-btn:not(.v-btn--outlined).success, .v-btn:not(.v-btn--outlined).error, .v-btn:not(.v-btn--outlined).warning, .v-btn:not(.v-btn--outlined).info {

}


.theme--dark.v-sheet {
   
    
    
}

.v-icon.v-icon{
  /* margin-right: 20px; */
}
</style>
