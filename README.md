
<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1">
<style>
body, html {
    height: 100%;
    margin: 0;
  }
  .bg {
    
    background-image: url("wat.jpg");
    
    height: 110%; 
   
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
  }
body {font-family: Arial;}
/* Style the tab */
.tab {
  overflow: hidden;
  border: 1px solid #ccc;
  background-color: #ccc;
}
/* Style the buttons inside the tab */
.tab button {
  background-color: white;
  float: left;
  border: none;
  outline: none;
  cursor: pointer;
  padding: 14px 16px;
  transition: 0.3s;
  font-size: 17px;
  font-color:black;
}
/* Change background color of buttons on hover */
.tab button:hover {
  background-color: #ccc;
}
/* Create an active/current tablink class */
.tab button.active {
  background-color: #ccc;
}
/* Style the tab content */
.tabcontent {
  display: none;
  color: black;
  padding: 6px 12px;
  border: 1px solid #ccc;
  border-top: none;
}
</style>
</head>
<body>

<h2>Ian's Water Polo Information</h2>


<div class="tab">
  <button class="tablinks" onclick="openCity(event, 'Waterpolo')">Water Polo</button>
  <button class="tablinks" onclick="openCity(event, 'Game video')">Game video</button>
  <button class="tablinks" onclick="openCity(event, 'resume')">Resume</button>
  <button class="tablinks" onclick="openCity(event, 'contact')">Contact</button>
  <button class="tablinks" onclick="openCity(event, 'coaches')">Coaches Contact</button>
  <button class="tablinks" onclick="openCity(event, 'about')">About</button>
</div>


<div id="Waterpolo" class="tabcontent">
  <h3>Water polo</h3>
  <p>My name is Ian Fry, I play water polo for Potomac Water Polo in Maryland.</p>
    <p><a href="https://seadevils.org/water-polo" target="_blank">My Team</a></p>
  
</div>
<div id="Game video" class="tabcontent">
    <p>Here is video of me at the 2018 Junior Olympic games<br/>Here are some of my game highlights:</p>
    <video width="320" height="240" controls>
                <source src="github/steal.mp4" type="video/mp4"> 
              </video>
    <video width="320" height="240" controls>
                <source src="github/shots.mp4" type="video/mp4"> 
              </video>
 </div>

<div id="resume" class="tabcontent">
  <h3>Here are my Water Polo acomplishments and events</h3>
  <p>
   2013 - 2018 JOs 
   <br/>
    2018 2nd place NJO 16u Invitational 
   <br/>
    2013-2016 ODP National Championships NEZ 
   <br/>
    2016 USA Waterpolo National Team Selection Camp 
    <br/>
    2018 and 2019 North VS. South Challenge Champions in North Carolina Tournament
    <br/>
    2017-2018, 2018-2019 High School Swim Team Virginia State Championships Meet
    <br/>
    2018 and 2019 George Mason Scolar Athlete 
   </p> 
</div>

<div id="contact" class="tabcontent">
  <h3>Contact information</h3>
  <p>Here is a list of my contact information. 
    <br/>
    Email: ianfrywaterpolo@gmail.com
    <br/>
    Phone #7035590270
    <br/>
    <a id="mySchool" href="https://gm.fccps.org">High School: George Mason</a>
    <br/> 
    City: Falls Church
    <br/>
      State: Virginia
    <br/>
     <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d24845.268559142238!2d-77.18982968260268!3d38.88605279807087!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x89b64b6e7a4663ad%3A0x6e536688973d9759!2sFalls+Church%2C+VA!5e0!3m2!1sen!2sus!4v1551505069642" width="600" height="450" frameborder="0" style="border:0" allowfullscreen></iframe>
    

  </p>
</div>
    <div id="coaches" class="tabcontent">
    <h4>Coaches information:</h4>
    <p> Potomac Waterpolo Club Head Coach Jonah Dowd
    <br/>
    Phone# 909-762-2740
    <br/>
    Email: jonahbdowd@gmail.com
    </p>
    
   <img src="github/jonah.jpeg" width="105" height="145">  
   </div>
   
<div id="about" class="tabcontent">
  <h3>About the website</h3>
  <p>
   2021 Graduation year
      <br/>
   Height: 6'1" 
      <br/>
   Weight: 200 (Lbs)
      <br/>
   Wing Span: 6' 7"
      <br/>
   50 (ft) Free Time: 24.63
      <br/>
   100 (ft) Free Time: 53.50
     <br/>
   50 (M)  BackStroke: 32.20
  <br/>   
This website was coded by me, Ian Fry. I wanted to have a website where I could post water polo highlights, and other information. However I wanted to do it in an interesting way, so I decided to code my own website using Html.</p>
</div>

<!-- below is the main needed stuff that i dont know much about, however i can put my needed information here as its below the tabs!-->
<div class="bg">
 

    
<script>
function openCity(evt, cityName) {
  var i, tabcontent, tablinks;
  tabcontent = document.getElementsByClassName("tabcontent");
  for (i = 0; i < tabcontent.length; i++) {
    tabcontent[i].style.display = "none";
  }
  tablinks = document.getElementsByClassName("tablinks");
  for (i = 0; i < tablinks.length; i++) {
    tablinks[i].className = tablinks[i].className.replace(" active", "");
  }
  document.getElementById(cityName).style.display = "block";
  evt.currentTarget.className += " active";
}
</script>
