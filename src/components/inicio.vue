<template>
    <div>
        
        <h1 style="">Inicio</h1>
        <p>Hola desde inicio</p>
        <b-button @click="navegarSiguiente" variant="primary">Siguiente</b-button>


        <p></p>
        <div>
            <b-jumbotron  bg-variant="info" text-variant="white" border-variant="dark">
              <template #header>Desarrollo web profesional - 8 A</template>
                <h1>Examen unidad 1</h1>
              <template #lead>
                Profesor: David Ivan Perez Torres
              </template>
          
              <hr class="my-4">
          
              <p>
                Alumno: Cesar Uriel Gonzalez Saldaña
              </p>
            </b-jumbotron>
          </div>

    </div>

    
</template>

<script>
import router from "@/router";

export default {
    methods: {
        navegarSiguiente() {
            router.push({ name: "formulario" });
        }
    },
items: [
        {
          text: "inicio",
          href: "Inicio",
        },
        {
          text: "formulario",
          active: true,
        },
      ],
      }
</script>

<style>

</style>