<template>
  <v-container id="home" class="cont">
    <div class="background"></div>
    <v-row justify="center" align="center" style="height: 100%;">
      <v-col></v-col>
      <v-col>
        <div style="text-align: center;">
          <img src="../assets/the_fun_du-trimmy.png">
        </div>
      </v-col>
      <v-col>
        <div style="display: flex; flex-direction: column;">
          <v-btn variant="outlined" href="#player" width="100px" class="mb-5">Playlist</v-btn>
          <v-btn variant="outlined" href="#album" width="100px" class="mb-5">Albums</v-btn>
          <v-btn variant="outlined" href="#schedule" width="100px" class="mb-5">Schedle</v-btn>
        </div>
      </v-col>
    </v-row>
  </v-container>
  
  <v-container id="player" class="block">
    
    <h1  class="title">Spotify Player</h1>
    <iframe style="border-radius:12px" 
      src="https://open.spotify.com/embed/playlist/0PWhB1LKuxePCF5F5p48yC?utm_source=generator&theme=0" 
      width="100%" height="80%" frameBorder="0" allow="autoplay; clipboard-write; encrypted-media; fullscreen; picture-in-picture" loading="lazy"></iframe>
  </v-container>
  
  <v-container class="cont">
      <div class="background1"></div>
  </v-container>
  
  <v-container id="album" class="block">
    <h1 class="title">Latest Album</h1>
    <v-row justify="center" align="center" style="height: 100%;">
      <v-col>
          <v-carousel
    height="400"
    hide-delimiters
    progress="red"
  >
    <v-carousel-item
      v-for="(slide, i) in slides"
      :key="i"
    >
      <v-sheet
        height="100%"
      >
        <div class="d-flex fill-height justify-center align-center">
          <div class="text-h2">
            {{ slide }}
          </div>
        </div>
      </v-sheet>
    </v-carousel-item>
  </v-carousel>
</v-col>
    </v-row>
    
  </v-container>
  
  <v-container class="parallax3">
    <h1 class="title">Parallax</h1>
  </v-container>
  
  <v-container id="schedule" class="block">
    <h1 class="title">Gig Schedule</h1>
  </v-container>
</template>
<script >
  export default {
    data () {
      return {
        slides: [
          'Looking Both Ways',
          'Holiday Special',
          'Jules Single',
          'Eyes - EP',
          'Hot Water Heater',
        ],
        shlides:[
          {}
        ]
      }
    },
  }
</script>
<style scoped>

.title{
  font-family: 'Sedgwick Ave Display', cursive;
  color: white;
  margin-bottom: 15px;
  margin-left: 65%;
  font-size: 20px;
}

.cont {
  height: 100vh;
 padding: 0;}
.cont img{
  height: 100%;

}
.background {
  background-image: url(../assets/laughing.jpg);
  background-size: cover;
  filter: blur(8px);
  position: absolute;
  width: 100%;
  height: 100%;
}
.background1 {
  background-image: url(../assets/sign.jpeg);
  background-size: cover;
  position: absolute;
  width: 100%;
  height: 100%;
}
.block {
  background-color: #181818;
  height: 110vh;
}
.block {
  background-color: #181818;
  height: 110vh;
}

.parallax2{
  background-color: grey;
  height: 60vh;
  max-width: 100vw;
}
.parallax3{
  background-color: grey;
  height: 60vh;
  max-width: 100vw;
}
</style>
