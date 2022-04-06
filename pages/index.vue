<template>
  <div>
    <b-navbar toggleable="lg" type="light" variant="info ">
      <b-navbar-brand href="#">Rick and Morty</b-navbar-brand>
      <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>
      <b-navbar-nav class="ml-auto">
        <b-collapse id="nav-collapse" is-nav>
          <b-navbar-nav>
            <b-nav-item to="/">INICIO</b-nav-item>
            <b-nav-item to="/buscar">BUSCAR</b-nav-item>
            <b-nav-item to="/about">ACERCA DE</b-nav-item>
          </b-navbar-nav>
        </b-collapse>
      </b-navbar-nav>
    </b-navbar>
    <CardComp :data-personajes="personajes" />
    
   </div>
</template>

<script>
export default {
  name: 'IndexPage',
  data() {
    return {
      personajes: [
        {
          id: 1,
          nombre: 'Morty',
          imagen: 'https://rickandmortyapi.com/api/character/avatar/2.jpeg',
        },
        {
          id: 2,
          nombre: 'Rick',
          imagen: 'https://rickandmortyapi.com/api/character/avatar/1.jpeg',
        },
        {
          id: 3,
          nombre: 'Summer',
          imagen: 'https://rickandmortyapi.com/api/character/avatar/3.jpeg',
        },
        {
          id: 4,
          nombre: 'Beth',
          imagen: 'https://rickandmortyapi.com/api/character/avatar/4.jpeg',
        },
        {
          id: 5,
          nombre: 'Jerry',
          imagen: 'https://rickandmortyapi.com/api/character/avatar/5.jpeg',
        },
      ],
    }
  },
}
</script>
