<template>
  <nav class="navbar navbar-expand-lg">
    <div class="navbar-container">
      <router-link class="navbar-brand" to="/">
        <span>
          <svg stroke="currentColor" fill="currentColor" stroke-width="0" version="1.1" viewBox="0 0 32 32" height="3rem" width="3rem" xmlns="http://www.w3.org/2000/svg"><path d="M13.632 5.289c-0.613 0.129-1.823 0.565-2.662 0.984-1.275 0.613-1.759 0.968-2.921 2.13s-1.517 1.646-2.13 2.921c-1.646 3.373-1.646 6.6 0 10.005 0.613 1.291 0.952 1.759 2.13 2.921 1.178 1.178 1.63 1.501 2.921 2.13 1.969 0.936 2.921 1.162 5.002 1.162s3.034-0.226 5.002-1.162c1.275-0.613 1.727-0.952 2.921-2.13 1.178-1.194 1.517-1.646 2.13-2.921 0.774-1.63 1-2.388 1.178-4.002l0.113-1h-3.195l-0.21 1.243c-1.017 6.471-8.907 9.069-13.587 4.47-3.792-3.712-2.969-10.005 1.678-12.732 0.871-0.516 2.63-1.049 3.437-1.049h0.532v-3.227l-0.597 0.016c-0.339 0-1.113 0.113-1.743 0.242zM14.213 9.645c-3.421 0.92-5.648 4.325-5.067 7.745 0.662 3.792 4.212 6.39 7.891 5.761 3.776-0.645 6.39-4.212 5.761-7.859-0.71-4.115-4.647-6.713-8.585-5.648z"></path></svg>
          Portfolio
        </span>
      </router-link>
      <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation" v-on:click="OnclickNavBar()">
        <!-- <span class="navbar-toggler-icon"></span> -->
        <svg stroke="currentColor" fill="currentColor" stroke-width="0" viewBox="0 0 448 512" height="1em" width="1em" xmlns="http://www.w3.org/2000/svg"><path d="M16 132h416c8.837 0 16-7.163 16-16V76c0-8.837-7.163-16-16-16H16C7.163 60 0 67.163 0 76v40c0 8.837 7.163 16 16 16zm0 160h416c8.837 0 16-7.163 16-16v-40c0-8.837-7.163-16-16-16H16c-8.837 0-16 7.163-16 16v40c0 8.837 7.163 16 16 16zm0 160h416c8.837 0 16-7.163 16-16v-40c0-8.837-7.163-16-16-16H16c-8.837 0-16 7.163-16 16v40c0 8.837 7.163 16 16 16z"></path></svg>
      </button>
      <div class="collapse navbar-collapse" id="navbarNav" v-show="NavBar">
        <ul class="navbar-nav ml-auto">
          <li class="nav-item">
            <a class="nav-link" href="#About">About</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#Skills">Skills</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#Experience">Experience</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#Projects">Projects</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#Education">Education</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#Contact">Contact</a>
          </li>
        </ul>
        <!-- <div class="clsGithub"><a href="#" target="_blank">Github Profile</a></div> -->
        <!-- <div class="clsCertifications"><a href="#" target="_blank">My Certifications</a></div> -->
      </div>
    </div>
  </nav>

  <div class="clsbodybg">
    <div id="About">
      <AboutPage />
    </div>

    <div class="cls-skills-experience-bg">
      <div id="Skills">
        <SkillsPage />
      </div>
      <div id="Experience">
        <ExperiencePage />
      </div>
    </div>
    
    <div id="Projects">
      <ProjectsPage />
    </div>

    <div class="cls-education-contact-bg">
      <div id="Education">
        <EducationPage />
      </div>
      <div id="Contact">
        <ContactPage />
      </div>
    </div>

    <div class="clsFooter">
      <footer>
        <h1>Pradeep</h1>
        <nav>
          <a href="#About">About</a>
          <a href="#Skills">Skills</a>
          <a href="#Experience">Experience</a>
          <a href="#Projects">Projects</a>
          <a href="#Education">Education</a>
          <a href="#Contact">Contact Me</a>
        </nav>
        <div class="clscontent">
          <a href="https://www.facebook.com/pradeep.selvaganapathy" target="display" class="clsSvg"><svg class="MuiSvgIcon-root MuiSvgIcon-fontSizeMedium css-vubbuv" focusable="false" aria-hidden="true" viewBox="0 0 24 24" data-testid="FacebookIcon"><path d="M5 3h14a2 2 0 0 1 2 2v14a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2V5a2 2 0 0 1 2-2m13 2h-2.5A3.5 3.5 0 0 0 12 8.5V11h-2v3h2v7h3v-7h3v-3h-3V9a1 1 0 0 1 1-1h2V5z"></path></svg></a>
          <a href="https://twitter.com/Pradeep_Selva24" target="display" class="clsSvg"><svg class="MuiSvgIcon-root MuiSvgIcon-fontSizeMedium css-vubbuv" focusable="false" aria-hidden="true" viewBox="0 0 24 24" data-testid="TwitterIcon"><path d="M22.46 6c-.77.35-1.6.58-2.46.69.88-.53 1.56-1.37 1.88-2.38-.83.5-1.75.85-2.72 1.05C18.37 4.5 17.26 4 16 4c-2.35 0-4.27 1.92-4.27 4.29 0 .34.04.67.11.98C8.28 9.09 5.11 7.38 3 4.79c-.37.63-.58 1.37-.58 2.15 0 1.49.75 2.81 1.91 3.56-.71 0-1.37-.2-1.95-.5v.03c0 2.08 1.48 3.82 3.44 4.21a4.22 4.22 0 0 1-1.93.07 4.28 4.28 0 0 0 4 2.98 8.521 8.521 0 0 1-5.33 1.84c-.34 0-.68-.02-1.02-.06C3.44 20.29 5.7 21 8.12 21 16 21 20.33 14.46 20.33 8.79c0-.19 0-.37-.01-.56.84-.6 1.56-1.36 2.14-2.23z"></path></svg></a>
          <a href="https://www.linkedin.com/in/pradeep-s-7ba81117b/" target="display" class="clsSvg"><svg class="MuiSvgIcon-root MuiSvgIcon-fontSizeMedium css-vubbuv" focusable="false" aria-hidden="true" viewBox="0 0 24 24" data-testid="LinkedInIcon"><path d="M19 3a2 2 0 0 1 2 2v14a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2V5a2 2 0 0 1 2-2h14m-.5 15.5v-5.3a3.26 3.26 0 0 0-3.26-3.26c-.85 0-1.84.52-2.32 1.3v-1.11h-2.79v8.37h2.79v-4.93c0-.77.62-1.4 1.39-1.4a1.4 1.4 0 0 1 1.4 1.4v4.93h2.79M6.88 8.56a1.68 1.68 0 0 0 1.68-1.68c0-.93-.75-1.69-1.68-1.69a1.69 1.69 0 0 0-1.69 1.69c0 .93.76 1.68 1.69 1.68m1.39 9.94v-8.37H5.5v8.37h2.77z"></path></svg></a>
          <a href="https://www.instagram.com/pradeep_selvaganapathy/" target="display" class="clsSvg"><svg class="MuiSvgIcon-root MuiSvgIcon-fontSizeMedium css-vubbuv" focusable="false" aria-hidden="true" viewBox="0 0 24 24" data-testid="InstagramIcon"><path d="M7.8 2h8.4C19.4 2 22 4.6 22 7.8v8.4a5.8 5.8 0 0 1-5.8 5.8H7.8C4.6 22 2 19.4 2 16.2V7.8A5.8 5.8 0 0 1 7.8 2m-.2 2A3.6 3.6 0 0 0 4 7.6v8.8C4 18.39 5.61 20 7.6 20h8.8a3.6 3.6 0 0 0 3.6-3.6V7.6C20 5.61 18.39 4 16.4 4H7.6m9.65 1.5a1.25 1.25 0 0 1 1.25 1.25A1.25 1.25 0 0 1 17.25 8 1.25 1.25 0 0 1 16 6.75a1.25 1.25 0 0 1 1.25-1.25M12 7a5 5 0 0 1 5 5 5 5 0 0 1-5 5 5 5 0 0 1-5-5 5 5 0 0 1 5-5m0 2a3 3 0 0 0-3 3 3 3 0 0 0 3 3 3 3 0 0 0 3-3 3 3 0 0 0-3-3z"></path></svg></a>
          <a href="mailto:pradeepselva2024@gmail.com" target="display" class="clsSvg"><svg class="MuiSvgIcon-root MuiSvgIcon-fontSizeMedium css-vubbuv" focusable="false" aria-hidden="true" viewBox="0 0 24 24" data-testid="MailIcon"><path d="M20 4H4c-1.1 0-1.99.9-1.99 2L2 18c0 1.1.9 2 2 2h16c1.1 0 2-.9 2-2V6c0-1.1-.9-2-2-2zm0 4-8 5-8-5V6l8 5 8-5v2z"></path></svg></a>
        </div>
        <p class="clsCopyRights">© 2024 Pradeep. All rights reserved.</p>
      </footer>
    </div>
  </div>
</template>

<script>
import AboutPage from './components/AboutPage.vue'
import ContactPage from './components/ContactPage.vue'
import EducationPage from './components/EducationPage.vue'
import ExperiencePage from './components/ExperiencePage.vue'
import ProjectsPage from './components/ProjectsPage.vue'
import SkillsPage from './components/SkillsPage.vue'

export default {
  name: 'App',
  components: {
    AboutPage,
    ContactPage,
    EducationPage,
    ExperiencePage,
    ProjectsPage,
    SkillsPage
  },
  data(){
    return{
      NavBar: false
    }
  },
  methods:{
    OnclickNavBar(){
      if(this.NavBar){
        this.NavBar = false
      }else{
        this.NavBar = true
      }
    }
  }
}
</script>