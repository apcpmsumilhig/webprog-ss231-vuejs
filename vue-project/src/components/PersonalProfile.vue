<template>
<div class = personalprofile>
    <!-- Header Tab -->
  <header class = "header">
    <div class = "header-holder">
      <div class = "header-text">
        <h1>Personal Profile Web page </h1>
      </div>
      <div class = "header-tabs">
        <div class= "tab"><h3> <a href = "">About Me </a></h3></div>
        <div class= "tab"><h3> <a href = "gallery">Picture Gallery</a></h3></div>
        <div class= "tab"><h3><a href = "">Contact Me!</a></h3></div>
  
      </div>
        
      
    </div>
    </header>

<!-- Profile Section -->
    <section class = profile>
      <div class = "profile-holder">
        <div class = "profile-container">
          <div class = "picture">
            <img src = "css/assets/profile.jpeg" id = "profile-picture" >
          </div>
          <div class = "intro">
            <h3>Hi I'm Paul Brian Sumilhig!</h3>
          </div>
          <div class = "profile-description">
            <h5>And you can find me here!</h5>
          </div>
          <div class = "socials-container">
            <div class = "socials-tab">
              <a href = "https://www.linkedin.com/in/paul-brian-sumilhig-531643320/" target="_blank">  LinkedIn  </a> 
            </div>
            <div class = "socials-tab">
              <a href = "https://github.com/apcpmsumilhig" target="_blank" > GitHub </a> 
            </div>
            <div class = "socials-tab">
              <a href = "https://www.facebook.com/normally.pol" target="_blank">  Facebook  </a> 
            </div>
          </div>
        </div>
      </div>
    </section>

  <!-- Main Content -->
  <div class="container">
    
    <main>
      <section class="main-content">
        <div class = "main-content-holder">

          <!--About Me-->

          <div class="content-container">
                <div class="content-text">
                    <h3>About Me</h3>
                    <p>I am a 2nd Year student currently in office as an officer for two organizations. Also inclined with analytics, statistics, as well as data science and similar topics.</p>
                </div>

                    <img src="css/assets/aboutme.png" class="main-content-image" alt="About Me Image">

            </div>
            <div class="content-container">
            <img class= "main-content-image" src= "css/assets/education.png" >
        <div class="content-text"><h3>Education</h3>  
        studied two different science high schools, one for Junior High School at <a href = "https://www.facebook.com/profile.php?id=100083844947925" target="_blank" title = "you can find my school here">Senator Renato Compañero Cayetano Memorial Science & Technology High School</a> and another one located at a different city for Senior High School at <a href="https://www.facebook.com/pcshs.edu" title = "you can find it here!">Pasig City Science High School</a> With Honors as a grade 12 student as well as a First Year College Student.<br>
    <br>
    <b>Achievements</b>
    <ul>
        <li>Was the Memberships head for Gaming Genesis</li>
        <li>Currently the Logistics Head for APC Microsoft Community</li>
        <li>Current President for Gaming Genesis</li>
    </ul>
</div>
</div>

<div class="content-container">
        <div class="content-text"><h3>Course</h3> 
        Currently studying as a Bachelor of Science in Computer Science specializing in Software Systems.
    </div> 
  
    <img class = "main-content-image" src = "https://www.apc.edu.ph/wp-content/uploads/2021/09/MicrosoftTeams-image-2-1024x670.jpg" alt= "I Study here!">
  </div>    
  <div class="content-container">
    <img class = "main-content-image" src="https://life360-website-cdn.life360.com/wp-content/uploads/sites/8/2024/03/AU-Homepage-Hero-image.png">
    <div class="content-text"><h3>IT Experience</h3>
        Had a <a href = "https://docs.google.com/document/d/1IbS4nP_PUzZyqjC5f1uV26DvfdhpoYD7kBNJlVIQJgo/edit?usp=sharing" target="_blank" title="here is our IMRADC">Mobile Development Project</a> that I developed alone for a Group Research Project using Java that works similarly to an Air Tag but has ways of communication to send information for different scenarios such as natural disasters as well as man-made scenarios
    </div>

    </div>
  
    <div class = "content-container">
      
    
        <div class="content-text"><h3>Hobbies & Interests</h3>
        As a person who doesn't really have anything to do in life, I commonly find myself doing these activities apart from looking at landscapes or "views" like the city lights in the evening.
        <br>
        <li>Reading</li>
        <ul>
            <li><a href="comick.io" target="_blank" title = "I read them here">Manga/Manhwa</a></li>
            <li><a href="comick.io" target="_blank" title  = "I also read them here">Webtoons</a></li>
        </ul>
        <li>Sleeping</li>
        <li>Cooking</li>
        <li>Photography</li>
        <li>Travelling</li>
        </div>
        <img class = "main-content-image" src="https://preview.redd.it/jgl8r3o4eog61.jpg?width=640&crop=smart&auto=webp&s=7740c69eaf34c8766b436bf40c3c6576a513832a">
      </div>
      <div class = "content-container">
        <img class = "main-content-image" src = "https://img.etimg.com/thumb/msid-105174440,width-650,height-488,imgsize-28384,resizemode-75/leodicaprio.jpg">
      
        <div class="content-text"><h3>Goals In Life / Dream</h3>
            to be so financially stable that I can spend on a day the average spending power of a person on a year.  
        </div>
        </div>
        </div>
      

        </section>
      
    </main>


    <div class="comments">
      <div id="app3">
          <form v-on:submit.prevent="sendComment">
              <p>
                  What would you like to say?<br>
                  <input type="text" required placeholder="Type it here" v-model="commentText">
              </p>
              <button type="submit">Send Comment</button>
          </form>
          <br>
  
          <div class="comment-list">
              <ul class="comment-list">
                  <li class="comment-item"
                      v-for="comment in commentPlace" 
                      v-bind:key="comment.name" 
                      v-show="!comment.found">
                      {{ comment.name }}
                  </li>
              </ul>
          </div>
      </div>
  </div>
    
    
    
  


  <!-- Footer -->
  <footer> <h4>Asia Pacific College WEBPROG SS231 
    <br><br>
    Developed by Paul Brian Sumilhig
    <br>
    Inspiration: <a href= "http://jpcs.apc.education" class="footerLink"> jpcs.apc.education</a> </h4>
  </footer>0
</div>
  </div>
</template>

<script></script>
<style>.container {
  display: grid;
  width: auto;
  background: rgba(255, 255, 255);
  background-attachment: fixed;
  background-position: center;
  background-size: cover;
}

/* Header */
.header {
  min-width: 100%;
  background: rgba(240, 240, 240);
  height: auto;
  padding-top: 2px;
  padding-bottom: 4px;
  background-image: linear-gradient(to bottom, rgba(255, 255, 255, 1) 0%, rgba(255, 255, 255, 1) 100%),
                    linear-gradient(to bottom, rgba(255, 255, 255, 1) 0%, rgba(231, 175, 65, 1) 100%);
  background-clip: content-box, padding-box;
  font-family: "Comfortaa", sans-serif;
}

.header-holder {
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: space-between;
}

.header-text {
  margin-left: 10px;
}

.header-tabs {
  display: flex;
  flex-direction: row;
}

.header-tabs > .tab {
  margin: 5px;
}

/* My Profile */
.profile {
  min-width: 100%;
  display: flex;
  flex-direction: column;
}

.profile-container {
  align-items: center;
}

.profile-holder {
  background-color: rgba(255, 255, 255, 0.475);
  align-items: center;
}

.picture {
  display: flex;
  align-items: center;
  justify-content: center;
}

.profile-holder > .profile-container {
  margin-top: 100px;
  margin-bottom: 100px;
  align-items: center;
}

#profile-picture {
  width: 150px;
  height: 200px;
}

.intro {
  text-align: center;
}

.profile-description {
  justify-content: center;
  text-align: center;
}

.socials-container {
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: center;
}

.socials-tab {
  border-right: 1px solid #35438c;
  border-left: 1px solid #35438c;
  padding: 5px;
}

.socials-container > .socials-tab {
  margin-left: 5px;
  margin-right: 5px;
}

/* Main Content */
.main-content {
  min-width: 100%;
  align-items: center;
  text-align: center;
}

.main-content-holder {
  margin: 100px auto;
  max-width: 800px;
}

body > footer {
  margin-top: 20px;
  min-width: 100%;
  max-width: 100%;
  background: #35438c;
  height: auto;
  padding-top: 20px;
  padding-bottom: 20px;
}

.content-text {
  text-align: justify;
  width: 30%;
  margin: 60px;
}

.content-container {
  display: flex;
  justify-content: center;
  align-items: center;
}

.main-content-image {
  width: 40%;
}

/* General Stuff */
body {
  margin: 0px auto;
  height: auto;
  font-family: "Comfortaa", sans-serif;
  background-repeat: no-repeat;
  background-attachment: fixed;
  background-position: center;
  background-size: cover;
}

footer {
  background-color: #35438c;
  text-align: center;
  min-width: 100%;
}

body > h1, h2, h3, h4, h5, h6 {
  font-family: "Comfortaa", sans-serif;
}

h4 {
  color: white;
  margin: 2px;
}

a:link, a:visited {
  text-decoration: none;
  color: #35438c;
}

a:hover {
  text-decoration: underline;
  color: rgba(231, 175, 65, 1);
}

a:active {
  text-decoration: underline;
  color: #35438c;
}

/* Media Queries for Responsiveness */
@media (max-width: 768px) {
  .header-holder {
    flex-direction: column; /* Stack header elements vertically */
  }

  .header-tabs {
    flex-direction: column; /* Stack tabs vertically */
  }

  .main-content-holder {
    margin: 20px; /* Reduce margins for smaller screens */
    width: 90%; /* Use more width on smaller screens */
  }

  .content-text {
    width: 90%; }}

    .appcontent img {
      width: 100px;
      height: auto; 
  }

li {
  color: black;
}
</style>