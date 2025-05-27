<script setup>
function scrollToTop() {
  window.scrollTo({
    top: 0,
    behavior: 'smooth',
  });
}
</script>

<template>
  <section class="container">
    <div class="row text-light">
      <div class="col-md-7">
        <div>
          <h1 id="topSection" class="display-1 cal-sans-regular header-color">Hello <br> I'm Roman Wernsing</h1>
        </div>
        <div class="montserrat-regular">
          <h3 class="fs-1">Full Stack Web Developer</h3>
          <p class="pt-2 fs-5">
            I'm a full stack web developer. I graduated from Boise CodeWorks in May of 2025, where I built a strong
            foundation in modern web technologies.
          </p>
          <p class="fs-5">
            I specialize in HTML, CSS, and JavaScript for creating responsive,
            user-friendly interfaces. I also have experience with backend development using REST APIs, Node.js, C#, and
            SQL to help websites work smoothly behind the scenes. My
            drive for continuous improvement in the web development field keeps me exploring new tools and frameworks to
            enhance
            both functionality
            and
            design. I thrive on solving problems and building clean, efficient code that brings ideas to life on the
            web.
          </p>
        </div>
      </div>
      <div class="col-md-5 d-none d-sm-none d-md-block">
        <div class="d-flex align-items-center justify-content-center" style="height: 100%">
          <img class="w-100 hero-img" src="https://cdn.pixabay.com/photo/2017/05/12/15/16/hexagon-2307350_1280.png"
            alt="hexagon symbol with element tag brackets">
        </div>
      </div>
      <div class="col-12">
        <div class="row justify-content-end">
          <div class="col-md-4">
            <div class="mt-5 mb-4">
              <h2 id="skillsSection" class="display-3 cal-sans-regular header-color text-end">Skills</h2>
            </div>
          </div>
          <div class="col-12 logo d-flex gap-4 justify-content-center flex-wrap align-items-center">
            <img src="../assets/img/html-logo.png" alt="Logo for HTML">
            <img src="../assets/img/css-logo.png" alt="Logo for CSS">
            <img src="../assets/img/js-logo.png" alt="Logo for Java Scripts">
            <img src="../assets/img/c-sharp-logo.png" alt="Logo for C#">
            <img src="https://www.myqnap.org/wp-content/uploads/nodejs-logo.gif" alt="Logo for Node.js">
            <img src="../assets/img/mySQL-logo.png" alt="Logo for MySQL">
            <img src="../assets/img/vue-logo.png" alt="Logo for Vue.js">
          </div>
        </div>
      </div>
      <div class="col-md-4">
        <div class="mt-5 mb-4">
          <h2 id="projectsSection" class="display-3 cal-sans-regular header-color">Projects</h2>
        </div>
      </div>
      <div class="col-12">
        <div class="row">
          <!-- <div class="col-md-6">
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
          </div> -->
          <!-- <div class="col-md-6">
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
          </div> -->
          <div class="col-md-6">
            <a href="https://tower.romanwernsing.org" target="_blank" title="Navigate to Tower">
              <div class="mb-5 project-box">
                <img class="w-100 project-img rounded-top-4" src="../assets/img/tower-screenshot.png"
                  alt="Screenshot of Tower">
                <div class="p-3 d-flex justify-content-between align-items-center">
                  <span class="text-light montserrat-regular fs-4">Tower</span>
                  <span class="w-50">Tower is a ticket and event managing app. I built it with Vue for the front-end
                    framework and Node.js and MongoDB for the backend and database. </span>
                </div>
              </div>
            </a>
          </div>
          <div class="col-md-6">
            <a href="https://keepr.romanwernsing.org" target="_blank" title="Navigate to Keepr">
              <div class="mb-5 project-box">
                <img class="w-100 project-img rounded-top-4" src="../assets/img/keepr-screen-shot.png"
                  alt="Screenshot of Keepr">
                <div class="p-3 d-flex justify-content-between align-items-center">
                  <span class="text-light montserrat-regular fs-4">Keepr</span>
                  <span class="w-50">Keepr is a photo based social media app, similar to Pintrest. I built it with vue
                    for the front-end .NET and MySQL for the backend and database.</span>
                </div>
              </div>
            </a>
          </div>
        </div>
      </div>
    </div>
    <div class="row justify-content-end">
      <div class="col-md-4">
        <div class="mt-5 mb-4">
          <h2 id="aboutSection" class="display-3 cal-sans-regular header-color text-end">About Me</h2>
        </div>
      </div>
      <div class="col-12">
        <div class="row justify-content-end">
          <div class="col-md-5 d-flex align-items-center justify-content-center">
            <div>
              <img class="w-100 profile-img my-5" src="../assets/img/profile_picture.jpeg" alt="">
            </div>
          </div>
          <div class="col-md-7">
            <div class="montserrat-regular text-light fs-5 text-end me-1">
              <p>
                I'm junior web developer based in Boise, ID. I started seriously coding in December 2024,
                but my interest in tech started early in my life. Thanks to a family member who passed down
                his love for coding and technology, that curiosity never really left me.
              </p>
              <p>
                I kicked things off with some Python courses online, but quickly realized I wanted to move faster. That
                led me to Boise CodeWorks, where I dove deep into web development and built a solid foundation. More
                importantly, I discovered that I love coding — the constant learning, the problem-solving, the "aha!"
                moments when something finally clicks.
              </p>
              <p>
                I'm looking for an internship or junior role in Frontend or Fullstack development. If you're looking for
                someone who's excited to learn, loves a good challenge, and brings a lot of energy, please
                feel free to reach out!
              </p>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="row">
      <div class="col-md-6">
        <div class="mt-5 mb-4">
          <h2 id="contactSection" class="display-3 cal-sans-regular header-color">Contact <br> Information</h2>
        </div>
      </div>
      <div class="col-12">
        <div class="row justify-content-evenly">
          <div class="col-12">
            <div class="text-light mb-5">
              <h3 class="fs-1 montserrat-regular">Have any questions?</h3>
              <p class="fs-5 montserrat-regular">Feel free to reach out!</p>
            </div>
          </div>
          <div class="col-md-3">
            <div class="mb-5">
              <p class="fs-4 text-light montserrat-regular">Email Address</p>
              <p class="text-light montserrat-regular">
                <a href="mailto:wernsingroman@gmail.com" title="Send an email to wernsingroman@gmail.com">
                  wernsingroman@gmail.com
                </a>
              </p>
            </div>
          </div>
          <div class="col-md-3">
            <div class="mb-5">
              <p class="fs-4 text-light montserrat-regular">LinkedIn Profile Link</p>
              <a href="https://www.linkedin.com/in/roman-wernsing-514b0a323" class="text-light montserrat-regular"
                target="_blank" title="Navigate to Roman Wernsing's LinkedIn">Roman Wernsing</a>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped lang="scss">
.logo img {
  height: 13dvh;
}

.logo {
  height: 40dvh;
}

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

a {
  text-decoration: none;
  color: white;
}


@media (max-width: 1200px) {
  .project-img {
    height: 38dvh;
  }

  .logo img {
    height: 10dvh;
  }

  .logo {
    height: 30dvh;
  }

}


@media (max-width: 991px) {
  .project-img {
    height: 28dvh;
  }

  .profile-img {
    height: 10dvh;
  }

  .logo img {
    height: 8dvh;
  }

  .logo {
    height: 20dvh;
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

.profile-img {
  aspect-ratio: 1/1;
  border-radius: 50%;
  height: 40dvh;
  object-fit: cover;
}
</style>
