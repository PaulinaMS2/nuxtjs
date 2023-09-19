<template>
  <div class="login">
      <h1>Bienvenidos a la app de Tareas</h1>
      <br>
      <v-sheet width="350" class="mx-auto">
          <v-form fast-fail @submit.prevent>
          <v-text-field
              label="Email"
              prepend-icon="mdi-email"
              type="email"
             
          ></v-text-field>

          <v-text-field
              label="Contraseña"
              type="password"
              prepend-icon="mdi-lock"
          ></v-text-field>
          ¿No tienes una cuenta? <nuxt-link to="/registro">Regístrate</nuxt-link>
          <v-btn color="primary" type="submit" block class="mt-2" to="/tareas">Iniciar sesión</v-btn>
          
          </v-form>
          
      </v-sheet>

  </div>

</template>

<style>

.login{
  width: 600px;
  margin:100px auto;
  padding: 40px;
  border-radius: 10px;
  box-shadow: 5px 5px 5px 5px rgba(54, 0, 59, 0.521) ;
  background-color: rgb(255, 255, 255);
  text-align: center;
  line-height: 1.5;
}

.login h1{
  margin: 0;
}


</style>

<script>
definePageMeta({
  layout: "blank",
});
</script>