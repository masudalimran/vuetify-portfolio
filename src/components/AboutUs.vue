<template>
  <v-container>
    <v-row>
      <v-col lg="6">
        <v-img
          lazy-src="../assets/loading.jpg"
          src="../assets/AboutUs/AboutUs.png"
          width="100%"
        ></v-img>
      </v-col>
      <v-col lg="6">
        <v-subheader class="text-h4 justify-center">About Us</v-subheader>
        <p>
          Lorem ipsum dolor sit, amet consectetur adipisicing elit. Eligendi
          modi officia eaque, cumque quidem ipsum ut totam alias tenetur rem.
        </p>
        <v-list>
          <v-list-item>
            <v-icon color="success" class="mr-3">mdi-check-all</v-icon>
            <v-list-item-subtitle>
              Lorem ipsum dolor sit amet.</v-list-item-subtitle
            >
          </v-list-item>
          <v-list-item>
            <v-icon color="success" class="mr-3">mdi-check-all</v-icon>
            <v-list-item-subtitle>
              Lorem ipsum dolor sit amet.</v-list-item-subtitle
            >
          </v-list-item>
          <v-list-item>
            <v-icon color="success" class="mr-3">mdi-check-all</v-icon>
            <v-list-item-subtitle>
              Lorem ipsum dolor sit amet.</v-list-item-subtitle
            >
          </v-list-item>
        </v-list>
        <p>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Iure adipisci
          non, reiciendis assumenda beatae, quos in consectetur eaque nesciunt
          cupiditate unde placeat laboriosam! Sunt minima illo nesciunt, saepe
          magnam perspiciatis rem veniam. Itaque doloremque quis veritatis quos
          ad tempore consectetur.
        </p>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {
    name: 'AboutUs'
};
</script>

<style lang="sass" scoped>
.v-subheader
    text-align: center
</style>