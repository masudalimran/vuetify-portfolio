<template>
  <v-container class="my-15">
    <v-row justify="center">
      <v-col lg="12" class="text-center">
        <v-subheader class="text-h4 justify-center">Portfolio</v-subheader>
        <p>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Doloremque
          quaerat repellendus harum tempore incidunt iste enim magni autem rem
          officia.
        </p>
      </v-col>
      <v-col lg="12">
        <div class="text-center">
          <v-chip @click="activePortfolio = 'webApp'" class="mx-5" :color="activePortfolio === 'webApp' ? 'success': ''">Web App</v-chip>
          <v-chip @click="activePortfolio = 'mobileApp'" class="mx-5" :color="activePortfolio === 'mobileApp' ? 'success': ''">Mobile App</v-chip>
          <v-chip @click="activePortfolio = 'deskApp'" class="mx-5" :color="activePortfolio === 'deskApp' ? 'success': ''">Desktop App</v-chip>
        </div>
      </v-col>
      <slot v-if="activePortfolio === 'webApp'">
        <v-col lg="3" v-for="(web, webIndex) in webApps" :key="webIndex">
            <v-card>
            <v-img
                :src="web.image"
                class="white--text align-end"
                gradient="to bottom, rgba(0,0,0,.1), rgba(0,0,0,.5)"
                height="200px"
            >
                <v-card-title>{{web.title}}</v-card-title>
            </v-img>
            </v-card>
        </v-col>
      </slot>
      <slot v-if="activePortfolio === 'mobileApp'">
        <v-col lg="3" v-for="(mobile, mobileIndex) in mobileApps" :key="mobileIndex">
            <v-card>
            <v-img
                :src="mobile.image"
                class="white--text align-end"
                gradient="to bottom, rgba(0,0,0,.1), rgba(0,0,0,.5)"
                height="200px"
            >
                <v-card-title>{{mobile.title}}</v-card-title>
            </v-img>
            </v-card>
        </v-col>
      </slot>
      <slot v-if="activePortfolio === 'deskApp'">
        <v-col lg="3" v-for="(desk, deskIndex) in desktopApps" :key="deskIndex">
            <v-card>
            <v-img
                :src="desk.image"
                class="white--text align-end"
                gradient="to bottom, rgba(0,0,0,.1), rgba(0,0,0,.5)"
                height="200px"
                lazy-src="../assets/loading.jpg"
            >
                <v-card-title>{{desk.title}}</v-card-title>
            </v-img>
            </v-card>
        </v-col>
      </slot>
    </v-row>
  </v-container>
</template>

<script>
export default {
  name: "Portfolio",
  data() {
      return {
          activePortfolio: 'webApp',
          webApps: [
              {title: 'Web App 1', image: 'https://picsum.photos/200/300?image=1'},
              {title: 'Web App 2', image: 'https://picsum.photos/200/300?image=2'},
              {title: 'Web App 3', image: 'https://picsum.photos/200/300?image=3'},
              {title: 'Web App 4', image: 'https://picsum.photos/200/300?image=4'},
              {title: 'Web App 5', image: 'https://picsum.photos/200/300?image=5'},
              {title: 'Web App 6', image: 'https://picsum.photos/200/300?image=6'},
              {title: 'Web App 7', image: 'https://picsum.photos/200/300?image=7'},
              {title: 'Web App 8', image: 'https://picsum.photos/200/300?image=8'},
          ], 
          mobileApps: [
              {title: 'Mobile App 0', image: 'https://picsum.photos/200/300?image=9'},
              {title: 'Mobile App 1', image: 'https://picsum.photos/200/300?image=10'},
              {title: 'Mobile App 2', image: 'https://picsum.photos/200/300?image=11'},
              {title: 'Mobile App 3', image: 'https://picsum.photos/200/300?image=12'},
              {title: 'Mobile App 4', image: 'https://picsum.photos/200/300?image=13'},
              {title: 'Mobile App 5', image: 'https://picsum.photos/200/300?image=14'},
              {title: 'Mobile App 6', image: 'https://picsum.photos/200/300?image=15'},
          ], 
          desktopApps: [
              {title: 'Desktop App 1', image: 'https://picsum.photos/200/300?image=16'},
              {title: 'Desktop App 2', image: 'https://picsum.photos/200/300?image=17'},
              {title: 'Desktop App 3', image: 'https://picsum.photos/200/300?image=18'},
              {title: 'Desktop App 4', image: 'https://picsum.photos/200/300?image=19'},
              {title: 'Desktop App 5', image: 'https://picsum.photos/200/300?image=20'},
          ] 
          
      }
  },
};
</script>

<style lang="sass" scoped>
</style>