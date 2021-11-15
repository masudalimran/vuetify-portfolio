<template>
  <v-footer padless>
    <v-col lg="12">
      <v-row justify="center">
        <v-col lg="4" class="text-center">
          <v-toolbar-title>Masud Al Imran</v-toolbar-title>
          <v-card-text>
            <v-btn
              v-for="icon in icons"
              :key="icon"
              class="mx-4 black--text"
              icon
            >
              <v-icon size="24px">
                {{ icon }}
              </v-icon>
            </v-btn>
          </v-card-text>
          <v-subheader
            >Lorem ipsum dolor sit amet consectetur adipisicing elit. Dolorem
            nemo officiis debitis aspernatur eum cumque culpa, delectus natus
            blanditiis repellendus!</v-subheader
          >
          <v-form>
            <v-text-field label="Email" outlined dense></v-text-field>
            <v-btn rounded color="success">Subscribe Us</v-btn>
          </v-form>
        </v-col>
      </v-row>
      <div class="mt-10">
          <v-divider></v-divider>
        <v-subheader>
            © Copyright Imon. All Rights Reserved {{ new Date().getFullYear() }} — <strong>Vuetify</strong>
            <v-spacer></v-spacer>
            <strong>Designed By Masud Al Imran</strong>
        </v-subheader>
      </div>
    </v-col>
  </v-footer>
</template>

<script>
export default {
  name: "Footer",
  data() {
    return {
      icons: ["mdi-facebook", "mdi-twitter", "mdi-linkedin", "mdi-instagram"],
    };
  },
};
</script>

<style lang="sass" scoped>
</style>