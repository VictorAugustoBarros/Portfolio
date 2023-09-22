<template>
  <section>
    <div class="container reveal">
      <h2>Caption</h2>
      <div class="text-container">
        <div class="text-box">
          <h3>Section Text</h3>
          <p class="glitch"  data-text="Lorem ipsum dolor sit amet consectetur adipisicing elit. Tempore eius molestiae perferendis eos provident vitae iste">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Tempore eius molestiae perferendis eos provident vitae iste.</p>
        </div>
      </div>
    </div>
  </section>
</template>

<script>

export default {
  name: 'SecondSection',
  created() {
    window.addEventListener("scroll", this.reveal);
  },
  methods: {
    reveal() {
      var reveals = document.querySelectorAll(".reveal");

      for (var i = 0; i < reveals.length; i++) {
        var windowHeight = window.innerHeight;
        var elementTop = reveals[i].getBoundingClientRect().top;
        var elementVisible = 150;

        if (elementTop < windowHeight - elementVisible) {
          reveals[i].classList.add("active");
        } else {
          reveals[i].classList.remove("active");
        }
      }
    }
  }
}
</script>

<style lang="scss">


section {
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
}

section:nth-child(1) {
  color: #e0ffff;
}

section .container {
  margin: 100px;
}

section h1 {
  font-size: 3rem;
  margin: 20px;
}

section h2 {
  font-size: 40px;
  text-align: center;
  text-transform: uppercase;
}

section .text-container {
  display: flex;
}

section .text-container .text-box {
  margin: 20px;
  padding: 20px;
}

section .text-container .text-box h3 {
  font-size: 30px;
  text-align: center;
  text-transform: uppercase;
  margin-bottom: 10px;
}

@media (max-width: 900px) {
  section h1 {
    font-size: 2rem;
    text-align: center;
  }

  section .text-container {
    flex-direction: column;
  }
}

.reveal {
  position: relative;
  transform: translateY(150px);
  opacity: 0;
  transition: 1s all ease;
}

.reveal.active {
  transform: translateY(0);
  opacity: 1;
}



</style>