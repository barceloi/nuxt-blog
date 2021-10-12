<template>
  <div class="home-page">
    <section class="intro">
      <h1>IBC</h1>
    </section>
    <section class="featured-posts">
      <PostPreview
        id="1"
        thumbnail="https://placedog.net/321"
        title="Just Javascript"
        previewText="Notas del curso"
      />
      <PostPreview
        id="2"
        thumbnail="https://placedog.net/221"
        title="Eloquent Javascript"
        previewText="Notas del libro"
      />
      <PostPreview
        id="3"
        thumbnail="https://placedog.net/421"
        title="CODE"
        previewText="Notas del libro"
      />
      <PostPreview
        id="4"
        thumbnail="https://placedog.net/721"
        title="CSS Art"
        previewText="Experimento"
      />
      <PostPreview
        id="5"
        thumbnail="https://placedog.net/821"
        title="Three.js"
        previewText="Experimento"
      />
      <PostPreview
        id="6"
        thumbnail="https://placedog.net/921"
        title="Memorias de Marco Aurelio"
        previewText="Notas del libro"
      />
      <PostPreview
        id="7"
        thumbnail="https://placedog.net/515"
        title="Naval Almanaque"
        previewText="Notas del libro"
      />
    </section>
  </div>
</template>

<script>
import PostPreview from "@/components/Posts/PostPreview";

export default {
  components: {
    PostPreview
  }
};
</script>

<style scoped>
.intro {
  height: 300px;
  position: relative;
  padding: 30px;
  box-sizing: border-box;
  background-image: url("~assets/images/hero-background.jpg");
  background-position: center;
  background-size: cover;
}

.intro h1 {
  position: absolute;
  top: 10%;
  left: 5%;
  width: 90%;
  font-size: 1.5rem;
  color: black;
  background-color: rgb(211, 211, 211);
  padding: 10px;
  border-radius: 10px;
  box-shadow: 3px 3px 3px black;
  box-sizing: border-box;
  border: 1px solid black;
}

@media (min-width: 768px) {
  .intro h1 {
    font-size: 2rem;
  }
}

.featured-posts {
  display: flex;
  padding: 20px;
  box-sizing: border-box;
  flex-wrap: wrap;
  align-items: center;
  justify-content: center;
}
</style>
