<template>
  <v-container class="my-15">
    <v-row justify="center">
      <v-col lg="12" class="text-center">
        <v-subheader class="text-h4 justify-center">Project</v-subheader>
        <p>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Doloremque
          quaerat repellendus harum tempore incidunt iste enim magni autem rem
          officia.
        </p>
      </v-col>
        <v-col lg="4" v-for="project in 3" :key="project">
        <v-card :loading="loading" class="mx-auto my-12" max-width="374">
          <v-img
            height="250"
            :src="`https://picsum.photos/500/300?image=${project * 5 + 10}`"
            :lazy-src="`https://picsum.photos/10/6?image=${project * 5 + 10}`"
          ></v-img>

          <v-card-title class="text-center">Web Development</v-card-title>

          <v-card-text>
            <div>
              Small plates, salads & sandwiches - an intimate setting with 12
              indoor seats plus patio seating.
            </div>
          </v-card-text>

          <v-divider class="mx-4"></v-divider>
          <v-card-actions>
            <v-btn color="success" rounded>View Details</v-btn>
            <v-spacer></v-spacer>
            <v-rating
              :value="4.5"
              color="amber"
              dense
              half-increments
              readonly
              size="14"
            ></v-rating>
          </v-card-actions>
        </v-card>
        </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {
  name: "Project",
};
</script>

<style lang="sass" scoped>
</style>