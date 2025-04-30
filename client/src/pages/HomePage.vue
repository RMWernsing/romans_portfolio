<script setup>


</script>

<template>
  <section class="container">
    <div class="row text-light">
      <div class="col-md-7">
        <div>
          <h1 class="display-1 cal-sans-regular header-color">Hello <br> I'm Roman Wernsing</h1>
        </div>
        <div class="montserrat-regular">
          <h3 class="fs-2">Full Stack Web Developer</h3>
          <p class="pt-2 fs-5">
            I'm a full stack web developer. I graduated from Boise CodeWorks in May of 2025, where I built a strong
            foundation in modern web technologies.
          </p>
          <p class="fs-5">
            I specialize in HTML, CSS, and JavaScript for creating responsive,
            user-friendly interfaces. I also have experience with backend development using REST APIs, Node.js, C#, and
            SQL to help websites work smoothly behind the scenes. My
            drive for continuous development in the web dev field keeps me exploring new tools and frameworks to enhance
            both functionality
            and
            design. I thrive on solving problems and building clean, efficient code that brings ideas to life on the
            web.
          </p>
        </div>
      </div>
      <div class="col-md-5 d-none d-sm-none d-md-block">
        <div class="d-flex align-items-center" style="height: 100%">
          <img class="w-100 hero-img" src="https://cdn.pixabay.com/photo/2017/05/12/15/16/hexagon-2307350_1280.png"
            alt="hexagon symbol with element tag brackets">
        </div>
      </div>
      <div class="col-md-4">
        <div class="mt-5">
          <h2 class="display-3 cal-sans-regular header-color">Projects</h2>
        </div>
      </div>
      <div class="col-12">
        <div class="row">
          <div class="col-md-6">
            <div class="mb-5 project-box">
              <img class="w-100 project-img rounded-top-4"
                src="https://images.unsplash.com/photo-1454165804606-c3d57bc86b40?q=80&w=2070&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D"
                alt="">
              <div class="p-3 d-flex justify-content-between align-items-center">
                <span class="text-light montserrat-regular fs-4">The Network</span>
                <span class="w-50">description of what this project is about, and how much i enjoyed working on it.
                  maybe the
                  technologies uses</span>
              </div>
            </div>
          </div>
          <div class="col-md-6">
            <div class="mb-5 project-box">
              <img class="w-100 project-img rounded-top-4"
                src="https://images.unsplash.com/photo-1454165804606-c3d57bc86b40?q=80&w=2070&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D"
                alt="">
              <div class="p-3 d-flex justify-content-between align-items-center">
                <span class="text-light montserrat-regular fs-4">Project U</span>
                <span class="w-50">description of what this project is about, and how much i enjoyed working on it.
                  maybe the
                  technologies uses</span>
              </div>
            </div>
          </div>
          <div class="col-md-6">
            <div class="mb-5 project-box">
              <img class="w-100 project-img rounded-top-4"
                src="https://images.unsplash.com/photo-1454165804606-c3d57bc86b40?q=80&w=2070&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D"
                alt="">
              <div class="p-3 d-flex justify-content-between align-items-center">
                <span class="text-light montserrat-regular fs-4">Tower</span>
                <span class="w-50">description of what this project is about, and how much i enjoyed working on it.
                  maybe the
                  technologies uses</span>
              </div>
            </div>
          </div>
          <div class="col-md-6">
            <div class="mb-5 project-box">
              <img class="w-100 project-img rounded-top-4"
                src="https://images.unsplash.com/photo-1454165804606-c3d57bc86b40?q=80&w=2070&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D"
                alt="">
              <div class="p-3 d-flex justify-content-between align-items-center">
                <span class="text-light montserrat-regular fs-4">Keepr</span>
                <span class="w-50">description of what this project is about, and how much i enjoyed working on it.
                  maybe the
                  technologies uses</span>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped lang="scss">
.header-color {
  background: #1C84CF;
  background: linear-gradient(85deg, rgba(202, 127, 240, 1) 0%, rgba(43, 72, 255, 1) 100%);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
}

.hero-img {
  filter: brightness(0) invert(1);

}

.project-img {
  height: 50dvh;
  object-fit: cover;
  object-position: center;
}

@media (max-width: 1200px) {
  .project-img {
    height: 38dvh;
  }

}

@media (max-width: 991px) {
  .project-img {
    height: 28dvh;
  }
}

@media (max-width: 767px) {
  .project-img {
    height: 38dvh;
  }
}

.project-box {
  border-radius: 18px;
  transition: box-shadow 300ms ease-in-out;
  transition: all 300ms ease-in-out;
  background-color: rgba(44, 44, 44, 0.575);
}

.project-box:hover {
  box-shadow: 0px 0px 30px lightgray;

}

.project-description {
  width: 20%;
}
</style>
