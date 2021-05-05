---
title: "Road-to-JS"
tags: ["HTML" , "CSS", "WebDev", "learning","university"]
date: 2021-05-05
---
Part of [[University-Studies]] branch.

## Road to JS (HTML & CSS)
In this semester, one of our subject is "JavaScript and its frameworks".
So I decided to start in the beggining, with a HTML&CSS crash course, since I didn't remember much of any of it 🤣

It was 10/10 decision beacuse I did learn extra shortcuts in the VSC.

<a href="https://youtu.be/D-h8L5hgW-w">This is the tutorial I'm using</a>

So, the HTML is used to create Web pages. We'll start with it to define <b>structure</b> of our page. CSS is for pretty things.

We start by typing ! and editor writes frist standard code for us, pretty handy eh? I didn't know about that before, but at least I know <b>now.</b>


	
```html
<!DOCTYPE html>
<html lang="en">
<head>
 	<meta charset\="UTF-8">
 	<meta http-equiv="X-UA-Compatible" content="IE=edge">
 	<meta name="viewport" content="width=device-width, initial-scale=1.0">
 <title>Document</title>
</head>
<body>

</body>
</html>

```

 One thing here that reqires our meddling is that we need to link our CSS file in the head.

```html
<link rel="stylesheet" href="css/main.css">
```

It looks like that.
Then we define the "body" of the page. General rule is: We go from top to bottom and left to right.
Finished HTML code:

```html
<!DOCTYPE html>
<html lang="en">
<head>
 	<meta charset="UTF-8">
 	<meta http-equiv="X-UA-Compatible" content="IE=edge">
 	<meta name="viewport" content="width=device-width, initial-scale=1.0">
 <title>Practice</title>
 <link rel="stylesheet" href="css/main.css">
</head>
<body>
 	<div class="navbar">
 		<div class="container">
 			<a href="#">Remember<span>That</span></a>

 			<img id="mobile-cta" class="mobile-menu" src="Assets/menu.svg" alt="Open navigation">
 			<nav>

 				<img id="mobile-exit" class="mobile-menu-exit" src="Assets/exit.svg" alt="Close navigation">

 				<ul class\="primary-nav">
 					<li class="current"><a href\="#">Home</a></li>
 					<li><a href="#">Features</a></li>
 					<li><a href="#">Pricing</a></li>
 				</ul>

 				<ul class="secondary-nav">
 					<li><a href="#">Contact</a></li>
 					<li class="go-premium-cta"><a href="#">Go Premium</a></li>
 				</ul>
 			</nav>
 		</div>
 	</div>

 	<section class="hero">
 		<div class="cointainer">
 			<div class="left-col">
 				<p class="subhead">It's Nitty &amp; Gritty</p>
 				<h1>A Task App That Dosen't Stink</h1>

 				<div class="hero-cta">
 					<a href="#" class="primary-cta">Try for free</a>
 					<a href="#" class="watch-video-cta">
 					<img src="Assets/watch.svg" alt="Watch a video">Watch a video
 					</a>

 				</div>
 			</div>

 			<img src="Assets/illustration.svg" class="hero-img" alt="illustration">
 		</div>
 	</section>

 	<section class="features-section">
 		<div class="container">
 			<ul>
 				<li>Unlimited Tasks</li>
 				<li\SMS Task Reminders</li>
 				<li>Confetti Explosions upon Task Completions</li>
 				<li>Social Media Announcements</li>
 				<li>Real Time Collaboration</li>
 				<li>Other awesome features</li>
 			</ul>
				
 			<img src="Assets/holding-phone.jpg" alt="Man holding a phone">
 		</div>
 	</section>

 	<section class="testimonials-section">
 		<div class="cointainer">
			<ul>
 				<li>
 					<img src="Assets/person.jpg" alt="Person">
 									<blockquote>"Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla"
					</blockquote>

 					<cite>- Jane Doe</cite>
 				</li>
 				<li>
 					<img src="Assets/person.jpg" alt="Person">
									<blockquote>"Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla"</blockquote>

 					<cite>- Jane Doe</cite>

 				</li>
				<li>
 					<img src="Assets/person.jpg" alt="Person">
									<blockquote>"Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla"</blockquote>

 					<cite>- Jane Doe</cite>

 				</li>
 			</ul>
 		</div>
 	</section>
 	<section class="contact-section">
 		<div class="cointainer">
 			<div class="contact-left">
 				<h2>Contact</h2>
				
 				<form action="">
 					<label for="name">Name</label>
 					<input type="text" id="name" name="name" placeholder="Your Name">
				
 					<label for="email">Email</label>
 					<input type="text" id="email" name="email">

 					<label for="message">Message</label>
 					<textarea name="message" id="message" cols="30" rows="10"></textarea>

  					<input type="submit" class="send-message-cta" value="Send message">
 				</form>
 			</div>
 			<div class="contact-right">
 				<iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d52871.866099047176!2d-118.43455339140397!3d34.08254393285968!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x80c2bc04d6d147ab%3A0xd6c7c379fd081ed1!2sBeverly%20Hills%2C%20CA%2C%20USA!5e0!3m2!1sen!2spl!4v1620164275033!5m2!1sen!2spl" width="600" height="450" style="border:0;" allowfullscreen="" loading="lazy"></iframe>
 		</div>
 	</div>
 </section> 
</body>
</html>
```

Some of most importantd things:
```Html
<div></div>
```
The `<div>` tag is used as a container for HTML elements - which is then styled with CSS or manipulated with JavaScript. It can be easily styled by using the class or id attribute.
```html
class="yourClass"
```
The `class` attribute is often used to point to a class name in a style sheet. It can also be used by a JavaScript to access and manipulate elements with the specific class name.
```html
id="myId"
```
The `id` attribute is a special snowflake, must be unique.

And now we have something like this:
<img src="https://raw.githubusercontent.com/MalgorzataSzopa/PictureHost/master/screen%20HTML.png" alt="page" style="width:100%"/>

<b>Well it definetly <i>needs</i> some CSS</b>😅
