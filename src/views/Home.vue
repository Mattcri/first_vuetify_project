<template>
  <div>
    <v-container>
      <v-row>
        <v-col
        v-for="(character, index) in characters"
        :key="index"
        cols="4"
        class="my-1"
        >
          <v-card max-width="350px">
            <v-img
            :src="character.image"
            aspect-ratio="1"
            >
            </v-img>
            <v-card-title>
              {{character.name}}
            </v-card-title>
            <v-card-text>
              Estado: {{character.status}}
              <br>
              Genero: {{character.gender}}
            </v-card-text>
          </v-card>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<script>
// @ is an alias to /src

export default {
  name: "Home",
  data: () => ({
    characters: [
      {
        id: 1,
        name: "Morty",
        image: "https://rickandmortyapi.com/api/character/avatar/2.jpeg",
        status: "Alive",
        gender: "Male"
      },
      {
        id: 2,
        name: "Rick",
        image: "https://rickandmortyapi.com/api/character/avatar/1.jpeg",
        status: "Alive",
        gender: "Male"
      },
      {
        id: 3,
        name: "Summer",
        image: "https://rickandmortyapi.com/api/character/avatar/3.jpeg",
        status: "Alive",
        gender: "Female"
      },
      {
        id: 4,
        name: "Beth",
        image: "https://rickandmortyapi.com/api/character/avatar/4.jpeg",
        status: "Alive",
        gender: "Female"
      },
      {
        id: 5,
        name: "Jerry",
        image: "https://rickandmortyapi.com/api/character/avatar/5.jpeg",
        status: "Alive",
        gender: "Male"
      },
    ],
  }),
};
</script>
