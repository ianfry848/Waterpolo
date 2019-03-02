
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
  background-color: #F3411A;
}
/* Style the buttons inside the tab */
.tab button {
  background-color: blue;
  float: left;
  border: none;
  outline: none;
  cursor: pointer;
  padding: 14px 16px;
  transition: 0.3s;
  font-size: 17px;
}
/* Change background color of buttons on hover */
.tab button:hover {
  background-color: #F3411A;
}
/* Create an active/current tablink class */
.tab button.active {
  background-color: #ccc;
}
/* Style the tab content */
.tabcontent {
  display: none;
  padding: 6px 12px;
  border: 1px solid #ccc;
  border-top: none;
}
</style>
</head>
<body>

<h2>Ian's waterpolo information</h2>
<!--<p>Click on the buttons inside the tabbed menu:</p>-->

<div class="tab">
  <button class="tablinks" onclick="openCity(event, 'waterpolo')">Waterpolo</button>
  <button class="tablinks" onclick="openCity(event, 'resumue')">Resumue</button>
  <button class="tablinks" onclick="openCity(event, 'contact')">Contact</button>
  <button class="tablinks" onclick="openCity(event, 'about')">About</button>
</div>


<div id="waterpolo" class="tabcontent">
  <h3>Waterpolo</h3>
  <p>this is a waterpolo website that I have made</p>
  <p>Here is me at the 2018 junior Olymipc games<br/>Here are some of my game highlights:</p>
          
            <video width="320" height="240" controls>
                <source src="github/steal.mp4" type="video/mp4"> 
              </video>
</div>

<div id="resumue" class="tabcontent">
  <h3>Here are my waterpolo acomplishments and events</h3>
  <p></p> 
</div>

<div id="contact" class="tabcontent">
  <h3>Contact information</h3>
  <p>Here is a list of my Contact information. 
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

<div id="about" class="tabcontent">
  <h3>About the website</h3>
  <p>This website was coded by me, Ian Fry. I wanted to have a website where I could post waterpolo highlights, and other information. However I wanted to do it in an interesting way, so I decided to make code my own website using Html</p>
</div>

<!-- below is the main needed stuff that i dont know much about, however i can put my needed information here as its below the tabs!-->
<div class="bg">
  <p>this is my website!<p/>
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

