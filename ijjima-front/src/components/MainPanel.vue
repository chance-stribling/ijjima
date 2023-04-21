<template>
  <v-container class="intro">
    <div class="background"></div>
    <v-row justify="center" align="center" style="height: 100%;">
      <v-col>
        <div style="text-align: center;">
          <img src="../assets/the_fun_du-trimmy.png">
        </div>
      </v-col>
    </v-row>
  </v-container>
  
  <v-container class="spotifyPlayer" >
    
    <h1 class="band">Spotify Player - put this in a div and make it a fixed footer</h1>
    <iframe style="border-radius:12px" 
      src="https://open.spotify.com/embed/playlist/0PWhB1LKuxePCF5F5p48yC?utm_source=generator&theme=0" 
      width="100%" height="80%" frameBorder="0" allow="autoplay; clipboard-write; encrypted-media; fullscreen; picture-in-picture" loading="lazy"></iframe>
  </v-container>
  
  <v-container class="parallax2">
    <h1 class="band">Parallax</h1>
  </v-container>
  
  <v-container class="album">
    <h1 class="band">Latest Album</h1>
  </v-container>
  
  <v-container class="parallax3">
    <h1 class="band">Parallax</h1>
  </v-container>
  
  <v-container class="schedule">
    <h1 class="band">Gig Schedule</h1>
  </v-container>
</template>
<script setup>

</script>
<style scoped>

.band{
  font-family: 'Sedgwick Ave Display', cursive;
  color: white;
  margin-bottom: 10px;
  margin-left: 25%;
}
.intro {
  height: 100vh;
  max-width: 100vw;
  padding: 0;
}
.intro img{
  height: 250px;

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
  padding: 0;
}
.spotifyPlayer {
  background-color: red;
  height: 90vh;
  max-width: 100vw;
}
.album {
  background-color: black;
  height: 105vh;
  max-width: 100vw;
}
.schedule {
  background-color: black;
  height: 100vh;
  max-width: 100vw;
}
.parallax1{
  background-color: grey;
  height: 60vh;
  max-width: 100vw;
  padding: 0;
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
