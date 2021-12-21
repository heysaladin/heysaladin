---
title: "Jumper"
---

<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1">
<style>
html {
  scroll-behavior: smooth;
}
body {
  margin: 0 auto;
  min-width: 360px;
  max-width: 360px;
  font-size: 28px;
  font-family: Arial, Helvetica, sans-serif;
}

.header {
  background-color: #f1f1f1;
  padding: 68px 0 0 0;
  text-align: center;
  height: 132px;
}

#navbar {
  overflow: auto;
  white-space: nowrap;
}

#navbar a {
  display: table-cell;
  color: white;
  text-align: center;
  padding: 4px 0px 2px;
  text-decoration: none;
}

#navbar a:hover {
}

/*
#navbar a {
  float: left;
  display: block;
  color: #f2f2f2;
  text-align: center;
  padding: 0px 2px;
  text-decoration: none;
  font-size: 17px;
}

#navbar a:hover {
  background-color: #ddd;
  color: black;
}
*/

#navbar a.active {
  color: white;
}

.content {
  padding: 0px;
}

.sticky {
  position: fixed;
  top: 0;
  width: 100%;
  min-width: 360px;
  max-width: 360px;
}

.sticky + .content {
  padding-top: 60px;
}

#top {
width: 100%;
height: 68px;
background: white;
position: fixed;
}

#navbar {
    display: flex;
    padding: 8px 0 16px;
}

#navbar a {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    padding: 2px 12px 8px;

    background: #FFFFFF;

    /* card shadow */
    box-shadow: 0px 1px 6px rgba(49, 53, 59, 0.12);
    border-radius: 8px;
    
    margin: 0px 8px;

    /* width: 72px;
    height: 74px; */
}

#navbar a.active {
    /* yellow / yellow-100 */
    background: #FFFAE6;

    /* yellow / yellow-400 */
    border: 1px solid #FF8B00;
    box-sizing: border-box;

    /* card shadow */
    box-shadow: 0px 1px 6px rgba(49, 53, 59, 0.12);
    border-radius: 8px;
}

#navbar a.active .text-nav {
    color: #FF8B00;
}

#navbar a .icon-nav {
    display:block; 
    width: 32px; 
    height: 32px; 
    padding: 8px;
}

#navbar a .text-nav {
    font-family: arial, sanserif;
    font-style: normal;
    font-weight: normal;
    font-size: 10px;
    line-height: 12px;

    /* or 120% */
    display: flex;
    align-items: center;
    text-align: center;

    /* Typography Default/Normal */
    color: rgba(49, 53, 59, 0.96);
}

#navbar a:nth-child(1) .icon-nav {
    background: url(./assets/styles/images/jumper/icon-1.png) no-repeat center center;
}
#navbar a:nth-child(1).active .icon-nav {
    background: url(./assets/styles/images/jumper/icon-1-a.png) no-repeat center center;
}

#navbar a:nth-child(2) .icon-nav {
    background: url(./assets/styles/images/jumper/icon-2.png) no-repeat center center;
}
#navbar a:nth-child(2).active .icon-nav {
    background: url(./assets/styles/images/jumper/icon-2-a.png) no-repeat center center;
}

#navbar a:nth-child(3) .icon-nav {
    background: url(./assets/styles/images/jumper/icon-3.png) no-repeat center center;
}
#navbar a:nth-child(3).active .icon-nav {
    background: url(./assets/styles/images/jumper/icon-3-a.png) no-repeat center center;
}

#navbar a:nth-child(4) .icon-nav {
    background: url(./assets/styles/images/jumper/icon-4.png) no-repeat center center;
}
#navbar a:nth-child(4).active .icon-nav {
    background: url(./assets/styles/images/jumper/icon-4-a.png) no-repeat center center;
}

#navbar a:nth-child(5) .icon-nav {
    background: url(./assets/styles/images/jumper/icon-5.png) no-repeat center center;
}
#navbar a:nth-child(5).active .icon-nav {
    background: url(./assets/styles/images/jumper/icon-5-a.png) no-repeat center center;
}

#navbar a:nth-child(6) .icon-nav {
    background: url(./assets/styles/images/jumper/icon-6.png) no-repeat center center;
}
#navbar a:nth-child(6).active .icon-nav {
    background: url(./assets/styles/images/jumper/icon-6-a.png) no-repeat center center;
}

</style>
</head>
<body>

<div id="top">
    <img class="h-auto" src="./assets/styles/images/jumper/header.png" alt="HeySaladin" />
</div>

<div class="header">
    <img class="h-auto" src="./assets/styles/images/jumper/banner.png" alt="HeySaladin" />
</div>

<div id="navbar">
  <a class="nav-item active" id="anchor-1" href="#section-1">
    <span class="icon-nav"></span>
    <span class="text-nav">Promo<br/>Terbaik</span>
  </a>
  <a class="nav-item" id="anchor-2" href="#section-2">
    <span class="icon-nav"></span>
    <span class="text-nav">Sesuai<br/>Budget</span>
  </a>
  <a class="nav-item" id="anchor-3" href="#section-3">
    <span class="icon-nav"></span>
    <span class="text-nav">Flash Sale</span>
  </a>
  <a class="nav-item" id="anchor-4" href="#section-4">
    <span class="icon-nav"></span>
    <span class="text-nav">Rilisan<br/>Spesial!</span>
  </a>
  <a class="nav-item" id="anchor-5" href="#section-5">
    <span class="icon-nav"></span>
    <span class="text-nav">Toko Pilihan</span>
  </a>
  <a class="nav-item" id="anchor-6" href="#section-6">
    <span class="icon-nav"></span>
    <span class="text-nav">Semua<br/>Event</span>
  </a>
</div>

<div class="content">
  <div id="section-1" class="section">
    <img class="h-auto" src="./assets/styles/images/jumper/section-1.png" alt="HeySaladin" />
   </div>
  <div id="section-2" class="section">
    <img class="h-auto" src="./assets/styles/images/jumper/section-2.png" alt="HeySaladin" />
   </div>
  <div id="section-3" class="section">
    <img class="h-auto" src="./assets/styles/images/jumper/section-3.png" alt="HeySaladin" />
   </div>
  <div id="section-4" class="section">
    <img class="h-auto" src="./assets/styles/images/jumper/section-4.png" alt="HeySaladin" />
   </div>
  <div id="section-5" class="section">
    <img class="h-auto" src="./assets/styles/images/jumper/section-5.png" alt="HeySaladin" />
   </div>
  <div id="section-6" class="section">
    <img class="h-auto" src="./assets/styles/images/jumper/section-6.png" alt="HeySaladin" />
   </div>
</div>


  <script src='https://cdnjs.cloudflare.com/ajax/libs/jquery/2.1.3/jquery.min.js'></script>
<script src='https://cdnjs.cloudflare.com/ajax/libs/waypoints/2.0.2/waypoints.min.js'></script>

<script>
window.onscroll = function() {myFunction()};

var navbar = document.getElementById("navbar");
var sticky = navbar.offsetTop;

var aNav = document.getElementById("navbar").querySelectorAll(".nav-item");

function myFunction() {
  if (window.pageYOffset + 68 >= sticky) {
    navbar.classList.add("sticky")
    navbar.style.background = "white"
    navbar.style.margin = "68px 0 0 0"
    aNav[0].style.flexDirection = "row"
    aNav[1].style.flexDirection = "row"
    aNav[2].style.flexDirection = "row"
    aNav[3].style.flexDirection = "row"
    aNav[4].style.flexDirection = "row"
    aNav[5].style.flexDirection = "row"
    aNav[0].style.padding = "0 10px 0 0"
    aNav[1].style.padding = "0 10px 0 0"
    aNav[2].style.padding = "0 10px 0 0"
    aNav[3].style.padding = "0 10px 0 0"
    aNav[4].style.padding = "0 10px 0 0"
    aNav[5].style.padding = "0 10px 0 0"
  } else {
    navbar.classList.remove("sticky");
    navbar.style.background = "white"
    navbar.style.margin = "0px 0 0 0"
    aNav[0].style.flexDirection = "column"
    aNav[1].style.flexDirection = "column"
    aNav[2].style.flexDirection = "column"
    aNav[3].style.flexDirection = "column"
    aNav[4].style.flexDirection = "column"
    aNav[5].style.flexDirection = "column"
    aNav[0].style.padding = "2px 12px 8px"
    aNav[1].style.padding = "2px 12px 8px"
    aNav[2].style.padding = "2px 12px 8px"
    aNav[3].style.padding = "2px 12px 8px"
    aNav[4].style.padding = "2px 12px 8px"
    aNav[5].style.padding = "2px 12px 8px"
  }
}
</script>
<!-- <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.3.1/jquery.min.js"></script> -->
<script>
$(document).ready(function(){

    $(window).on('scroll', function() {
    console.log( $(this).scrollTop() );
});

  // Add smooth scrolling to all links
  $("a").on('click', function(event) {

    // Make sure this.hash has a value before overriding default behavior
    if (this.hash !== "") {
      // Prevent default anchor click behavior
      event.preventDefault();

      // Store hash
      var hash = this.hash;

      // Using jQuery's animate() method to add smooth page scroll
      // The optional number (800) specifies the number of milliseconds it takes to scroll to the specified area
      $('html, body').animate({
        scrollTop: $(hash).offset().top - 160
      }, 100, function(){

        // Add hash (#) to URL when done scrolling (default click behavior)
        window.location.hash = hash;
      });
    } // End if
  });
});
</script>


<script>
// Add active class to the current button (highlight it)
var header = document.getElementById("navbar");
var btns = header.getElementsByClassName("nav-item");
for (var i = 0; i < btns.length; i++) {
  btns[i].addEventListener("click", function() {
  var current = document.getElementsByClassName("active");
  current[0].className = current[0].className.replace(" active", "");
  this.className += " active";
  });
}
</script>

<script>
// $('document').ready(function(){

// 	var s = $('.section');
// 	var nav = $('#navbar a');
// 	s.waypoint({
// 		handler: function(direction){
// 			var active = $(this);
// 			if(direction == 'up')
// 				active = active.prev();
// 			var active_link = $('#navbar a[href="#'+active.attr('id')+'"]');
			
		
// 			nav.parent().removeClass('active');
// 			active_link.parent().addClass('active');
// 		},
// 		offset: '35%'
// 	});

// });
// (function($){
// 	$('.navbar a').click(function(){
// 		console.log($(this).attr('id'));
// 		//$('body').scrollTop($(this).attr('id'));
// 	});
// });

// var waypoint = new Waypoint({
//   element: document.getElementById('.navbar'),
//   handler: function(direction) {
//     notify(this.id + ' hit')
//   }
// })


//Default active on home
// $('#anchor-1').addClass("active");


/*
Using jquery waypoints to change active on scroll
*/

// $('#section-2').waypoint(function() {
//   $("#navbar").children().removeClass("active");
//   $("#anchor-2").addClass("active");
// }, { offset: 1460 });


// $('#section-3').waypoint(function() {
//   $("#navbar").children().removeClass("active");
//   $("#anchor-3").addClass("active");
// }, { offset: 2324 });


// $('#section-4').waypoint(function() {
//   $("#navbar").children().removeClass("active");
//   $("#anchor-4").addClass("active");
// }, { offset: 3588 });


// $('#section-5').waypoint(function() {
//   $("#navbar").children().removeClass("active");
//   $("#anchor-5").addClass("active");
// }, { offset: 4308 });


// $('#section-6').waypoint(function() {
//   $("#navbar").children().removeClass("active");
//   $("#anchor-6").addClass("active");
// }, { offset: 5700 });


// $('#section-1').waypoint(function() {
//   $("#navbar").children().removeClass("active");
//   $("#anchor-1").addClass("active");
// }, { offset: 100 });

// $('#anchor-4').waypoint(function() {
//   $("#navbar a").children().removeClass("active");
//   $("#anchor-4").addClass("active");
// }, { offset: 101 });

// $('#navbar a').waypoint(function() {
//   $("#navbar a").children().removeClass("active");
//   $("#anchor-1").addClass("active");
// }, { offset: 0 });

// $('#section-2').waypoint(function() {
//   $(".to-top").addClass("visible");
// }, { offset: 100 });

// $('#section-1').waypoint(function(event, direction) {
//   $(".to-top").removeClass("visible");
// }, { offset: 30 });

</script>

</body>
</html>
