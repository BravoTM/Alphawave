<template style="background-color:blue">
  <div class="container">
    <div class="anime-carousel-container">
      <h2 class="anime-carousel-title">Anime Carousel</h2>
      <div class="anime-carousel">
        <div class="anime-card">
          <img src="./../public/download (1).jpg" alt="Anime 1" class="anime-image" />
          <h3 class="anime-title">Anime 1</h3>
        </div>
        <div class="anime-card">
          <img src="https://via.placeholder.com/150" alt="Anime 2" class="anime-image" />
          <h3 class="anime-title">Anime 2</h3>
        </div>
        <div class="anime-card">
          <img src="https://via.placeholder.com/150" alt="Anime 3" class="anime-image" />
          <h3 class="anime-title">Anime 3</h3>
        </div>
        <div class="anime-card">
          <img src="https://via.placeholder.com/150" alt="Anime 4" class="anime-image" />
          <h3 class="anime-title">Anime 4</h3>
        </div>
      </div>
    </div>
    <div class="anime-list-container">
      <h2 class="anime-list-title">Anime List</h2>
      <div class="anime-list">
        <div class="anime-item" v-for="anime in animeList" :key="anime.id">
          <img :src="anime.image" :alt="anime.title" class="anime-image" />
          <h3 class="anime-title">{{ anime.title }}</h3>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      animeList: [
        { id: 1, title: "Anime 1", image: "./../public/download (1).jpg" },
        { id: 2, title: "Anime 2", image: "https://via.placeholder.com/100" },
        { id: 3, title: "Anime 3", image: "https://via.placeholder.com/100" },
        { id: 4, title: "Anime 4", image: "https://via.placeholder.com/100" },
        { id: 5, title: "Anime 5", image: "https://via.placeholder.com/100" },
        { id: 6, title: "Anime 6", image: "https://via.placeholder.com/100" },
        { id: 7, title: "Anime 7", image: "https://via.placeholder.com/100" },
        { id: 8, title: "Anime 8", image: "https://via.placeholder.com/100" },
        { id: 9, title: "Anime 9", image: "https://via.placeholder.com/100" },
        { id: 10, title: "Anime 10", image: "https://via.placeholder.com/100" },
      ],
    };
  },
};
</script>

