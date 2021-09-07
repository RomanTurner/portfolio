<template>
  <div class="about-container">
    <div class="about-card">
      <iframe
        width="100%"
        height="100%"
        src="https://www.youtube.com/embed/BAtwf7KsuJg"
        title="YouTube video player"
        frameborder="0"
        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
        allowfullscreen
      ></iframe>
    </div>
    <div class="about-card">
      <iframe
        width="100%"
        height="100%"
        src="https://www.youtube.com/embed/Bzmh792Q20Y"
        title="YouTube video player"
        frameborder="0"
        allow="accelerometer; autoplay=1; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
        allowfullscreen
      ></iframe>
    </div>
  </div>
</template>

<style scoped>
.about-container {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  flex-wrap: wrap;
}
.about-card {
  width: 700px;
  height: 400px;
  padding: 10px;
  margin: 10px;
  margin-top: 10px;
  background: white;
  box-shadow: 0 2px 2px 0 rgba(0, 0, 0, 0.14), 0 1px 5px 0 rgba(0, 0, 0, 0.12),
    0 3px 1px -2px rgba(0, 0, 0, 0.2);
}

h4 {
  margin: 5px;
}
</style>
