<template>
  <div class="container">
    <h1>Alex Shuey</h1>
    <h2>Full Stack Software Engineer</h2>
    <div class="social-links">
      <a href="mailto:alex@alexshuey.com" class="social-link">
        <email-icon></email-icon>
      </a>
      <a href="https://github.com/ashuey" class="social-link">
        <github-icon></github-icon>
      </a>
      <a href="https://www.linkedin.com/in/ashuey/" class="social-link">
        <linkedin-icon></linkedin-icon>
      </a>
    </div>

    <a href="resume.pdf" class="button">
      Download Resume
    </a>
  </div>
</template>

<script>
import GithubIcon from "~/components/GithubIcon";
import LinkedinIcon from "~/components/LinkedinIcon";
import EmailIcon from "~/components/EmailIcon";

export default {
  components: {EmailIcon, LinkedinIcon, GithubIcon}
}
</script>

<style scoped>
img {
  border-radius: 50%;
  width: 150px;
  height: auto;
  border-style: solid;
  border-width: 3px;
  border-color: #bbb;
}
.container {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  min-height: 100vh;
}

h1 {
  font-size: 3rem;
  letter-spacing: -.025em;
  font-weight: 800;
  margin: 0 0 0.5rem;
}

h2 {
  font-size: 1.25rem;
  font-weight: 300;
  color: #bbb;
  margin: 0 0 2rem;
}

.social-links {
  display: flex;
  margin-bottom: 3rem;
}

.social-link {
  color: currentColor;
  display: block;
  margin-left: 0.5rem;
  margin-right: 0.5rem;
}

.social-link svg {
  height: 32px;
  width: auto;
}

.button {
  padding: 0.5rem 1rem;
  border-radius: .25rem;
  font-weight: 300;
  border-style: solid;
  border-width: 1px;
  border-color: white;
  color: white;
  text-decoration: none;
  transition: color .15s ease-in-out, background-color .15s ease-in-out;
}

.button:hover {
  background-color: white;
  color: #444;
}
</style>
