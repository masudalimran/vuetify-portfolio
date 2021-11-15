<template>
  <v-container class="my-15">
    <v-row justify="center">
      <v-col lg="12" class="text-center">
        <v-subheader class="text-h4 justify-center">Contact Us</v-subheader>
        <p>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Doloremque
          quaerat repellendus harum tempore incidunt iste enim magni autem rem
          officia.
        </p>
      </v-col>
      <v-col lg="6">
        <iframe
          src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d29202.132933343113!2d90.35860293189815!3d23.80911646185397!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x3755c72537359ad1%3A0xfe2b9ddbb9daf23b!2sBISMIB%20TECHNOLOGY!5e0!3m2!1sen!2sbd!4v1636897845974!5m2!1sen!2sbd"
          width="100%"
          height="100%"
          style="border: 0"
          allowfullscreen=""
          loading="lazy"
        ></iframe>
      </v-col>
      <v-col lg="6">
        <v-form ref="form" lazy-validation>
          <v-text-field
            v-model="contactInfo.name"
            :counter="40"
            label="Name"
            required
          ></v-text-field>

          <v-text-field
            v-model="contactInfo.email"
            label="E-mail"
            required
          ></v-text-field>

          <v-textarea
            v-model="contactInfo.message"
            outlined
            name="input-7-4"
            label="Message"
            :counter="200"
          ></v-textarea>

          <v-btn color="success" class="mr-4"> Send </v-btn>
        </v-form>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {
  name: "ContactUs",
  data() {
    return {
      contactInfo: {},
    };
  },
};
</script>

<style lang="sass" scoped>
</style>