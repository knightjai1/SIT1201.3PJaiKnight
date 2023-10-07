<template>
  <section class="about-me-page">
    <div class="profile-image">
      <img src="../assets/My_Picture.jpeg" alt="Picture of me and my brother Adam(I am on the right)" class="projectImage">
    </div>
    <div class="about-content">
      <h1>About Me</h1>
      <p>Hello! My name is Jai, and I am currently studying a Bachelor of IT, majoring in Cybersecurity. 
        I am currently in year 2 of this course, and about 2 years away from graduation.
        I enjoy hanging out with friends and family, playing games and going to the gym in my free time. 
        See below my downloadable resume.</p>
    
      <button class="download-btn" @click="downloadFile">Download My Resume</button>
      <p>Thanks! Feel free to <a href="mailto:sample-email@example.com"> Reach out</a>!</p>
    </div>
  </section>
</template>

<script>
export default {
    methods: {
        downloadFile() {
            const filePath = '../cv.pdf';

            const link = document.createElement('a');
            link.href = filePath;
            link.setAttribute('download', 'MyCV.pdf');
            link.style.display = 'none';

            document.body.appendChild(link);
            link.click();

            document.body.removeChild(link);
        },
    },
};
</script>


<style>
@media (min-width: 1024px) {
  .about {
    min-height: 100vh;
    display: flex;
    align-items: center;
  }
}
</style>
