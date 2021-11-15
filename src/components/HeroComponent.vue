<template>
  <v-container class="pt-15">
    <v-row>
      <v-col lg="6" class="pt-16">
        <h2 class="hero-head">Welcome to my portfolio</h2>
        <p class="hero-para">
          Lorem ipsum dolor sit amet, consectetur adipisicing elit. Animi dolor,
          dolore facilis illum iusto molestias mollitia ratione saepe tempore
          voluptatibus!
        </p>
        <v-btn color="success" class="white--text mr-10">Get started</v-btn>
        <v-btn color="indigo" class="white--text" rounded>
          <v-icon>mdi-play-circle</v-icon>Watch Video
        </v-btn>
      </v-col>
      <v-col lg="6">
        <v-img
          lazy-src="../assets/loading.jpg"
          src="../assets/HeroComponent/heroComponent_main.jpg"
          width=100%
        ></v-img>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {
  name: "HeroComponent",
};
</script>

<style lang="sass" scoped>
h2.hero-head
    font-size: 60px
    font-weight: bold
    font-family: cursive
    color: #444
    p.hero-para
        font-size: 19px
        font-family: cursive
        margin: 32px 0px
        color: #444444ba
</style>
