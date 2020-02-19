1. General CSS

```
* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

body {
  font-family: "Segoe UI", Tahoma, Geneva, Verdana, sans-serif;
  background: #fff;
  font-size: 15px;
  color: #000;
  line-height: 1.5;
}

a {
  color: #262626;
  text-decoration: none;
}

ul {
  list-style: none;
}

.container {
  width: 90%;
  max-width: 1100px;
  margin: auto;
}
```

2. nav bar

```
   <nav class="main-nav">
   <img src="img/logo.png" alt="Microsoft" class="logo" />
   <ul class="main-menu">
   <li><a href="#">Office</a></li>
   <li><a href="#">Windows</a></li>
   <li><a href="#">Surface</a></li>
   <li><a href="#">Xbox</a></li>
   <li><a href="#">Deals</a></li>
   <li><a href="#">Support</a></li>
   </ul>
   <ul class="right-menu">
   <li>
   <a href="#">
   <i class="fas fa-search"></i>
   </a>
   </li>
   <li>
   <a href="#">
   <i class="fas fa-shopping-cart"></i>
   </a>
   </li>
   </ul>
   </nav>
```

```
.main-nav {
display: flex;
align-items: center;
height: 60px;
padding: 20px 0;
font-size: 13px;
justify-content: space-between;
}

.main-nav .logo {
width: 110px;
}

.main-nav ul {
display: flex;
}

.main-nav ul li {
padding: 0 10px;
}

.main-nav ul li a {
padding-bottom: 2px;
}

.main-nav ul li a:hover {
border-bottom: 2px solid #262626;
}

.main-nav ul.main-menu {
flex: 1;
margin-left: 20px;
}
```

3.  Showcase

    <!-- ShowCase -->
    <header class="showcase">
      <h2>Surface Deals</h2>
      <p>
        Select Surfaces are on sale now - save while supplies last
      </p>
      <a href="#" class="btn"> Shop Now <i class="fas fa-chevron-right"></i> </a>
    </header>

/_ Showcase _/

.showcase {
width: 100%;
height: 400px;
background: url("./img/slide1.png") no-repeat center center/cover;
display: flex;
flex-direction: column;
align-items: center;
text-align: center;
justify-content: flex-end;
padding-bottom: 50px;
margin-bottom: 20px;
}

.showcase h2,
.showcase p {
margin-bottom: 10px;
}

.showcase .btn {
margin-top: 20px;
}

4.  Home Cards

          <!-- Home Cards 1 -->
          <section class="home-cards">
          <div>
          <img src="./img/card1.png" alt="" />
          <h3>New Surface Pro 7</h3>
          <p>See how Katie Sowers, Asst. Coach for the 49ers, uses Surface Pro 7 to put her plans into play.</p>
          <a href="#">Learn More <i class="fas fa-chevron-right"></i></a>
          </div>
          <div>
          <img src="./img/card2.png" alt="" />
          <h3>New Surface Laptop 3</h3>
          <p>
          Express yourself powerfully with a thin, light, and elegant design, faster performance, and up to 11.5 hours battery life.
          </p>
          <a href="#">Learn More <i class="fas fa-chevron-right"></i></a>
          </div>
          <div>
          <img src="./img/card3.png" alt="" />
          <h3>Save $150 + free controller</h3>
                 <p>
                   Buy an Xbox One X console and double your fun with a free select extra controller. Starting at $349.
          </p>
          <a href="#">Learn More <i class="fas fa-chevron-right"></i></a>
          </div>
          <div>
          <img src="./img/card4.png" alt="" />
          <h3>The new Microsoft Edge</h3>
          <p>
          Expect more. World class performance, with more privacy, more productivity, and more value.
          </p>
          <a href="#">Learn More <i class="fas fa-chevron-right"></i></a>
          </div>
          </section>


    /_ Home cards _/
    .home-cards {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    grid-column-gap: 20px;
    margin-bottom: 40px;
    }

.home-cards img {
width: 100%;
margin-bottom: 20px;
}

.home-cards h3 {
margin-bottom: 5px;
}

.home-cards a {
display: inline-block;
padding-top: 10px;
color: #0067b8;
text-transform: uppercase;
font-size: bold;
}

.home-cards a:hover i {
margin-left: 10px;
}

5. Xbox
   /_ Xbox Styling _/

.xbox {
height: 350px;
width: 100%;
background: url("./img/xbox.png") no-repeat center center/cover;
margin-bottom: 20px;
}

.xbox .content {
width: 40%;
padding: 50px 0 0 30px;
}

.xbox p {
margin: 10px 0 20px;
}

      <!-- Xbox Section -->
      <section class="xbox">
        <div class="content">
          <h2>Xbox Game Pass Ultimate</h2>
          <p>
            Xbox Game Pass Ultimate Xbox Live Gold and over 100 high-quality console and PC games. Play together with friends and
            discover your next favorite game.
          </p>
          <a href="#" class="btn"> Join Now <i class="fas fa-chevron-right"></i> </a>
        </div>
      </section>

6. Home Cards two

   <!-- Home cards 2 -->
   <section class="home-cards">
     <div>
       <img src="https://i.ibb.co/zVqhWn2/card5.png" alt="" />
       <h3>Microsoft Teams</h3>
       <p>
         Unleash the power of your team.
       </p>
       <a href="#">Shop Now <i class="fas fa-chevron-right"></i></a>
     </div>
     <div>
       <img src="https://i.ibb.co/mGZcxcn/card6.jpg" alt="" />
       <h3>Unlock the power of learning</h3>
       <p>
         Get students future-ready with Windows 10 devices. Starting at $219.
       </p>
       <a href="#">Shop Now <i class="fas fa-chevron-right"></i></a>
     </div>
     <div>
       <img src="https://i.ibb.co/NpPvVHj/card7.png" alt="" />
       <h3>Windows 10 Enterprise</h3>
       <p>
         Download the free 90-day evaluation for IT professionals.
       </p>
       <a href="#">Download Now <i class="fas fa-chevron-right"></i></a>
     </div>
     <div>
       <img src="https://i.ibb.co/LkP4L5T/card8.png" alt="" />
       <h3>Explore Kubernetes</h3>
       <p>
         Learn how Kubernetes works and get started with cloud native app development today.
       </p>
       <a href="#">Get Started <i class="fas fa-chevron-right"></i></a>
     </div>
   </section>

7. Carbon

<!-- Carbon -->

      <section class="carbon dark">
        <div class="content">
          <h2>Commiting To Carbon Negative</h2>
          <p>
            Microsoft will be carbon negative by 2030 and by 2050 we will remove all carbon the company has emitted since it was
            founded in 1975
          </p>
          <a href="#" class="btn"> Learn More <i class="fas fa-chevron-right"></i> </a>
        </div>
      </section>

.dark {
color: #fff;
}

.dark .btn {
background: #f4f4f4;
color: #333;
}

.xbox p,
.carbon p {
margin: 10px 0 20px;
}

/_ Carbon _/

.carbon {
height: 350px;
width: 100%;
background: url("./img/carbon.jpg") no-repeat center center/cover;
}

.carbon .content {
width: 55%;
padding: 100px 0 0 30px;
}

6. Follow

   <!-- Follow -->

   <section class="follow">
     <p>Follow Microsoft</p>
     <a href="https://facebook.com"><img src="./img/social-fb.png" alt="Facebook"/></a>
     <a href="https://twitter.com"><img src="./img/social-twitter.png" alt="Twitter"/></a>
     <a href="https://linkedin.com"><img src="./img/social-linkedin.png" alt="Linkedin"/></a>
   </section>

/_ Follow _/

.follow {
display: flex;
align-items: center;
justify-content: flex-start;
margin: 30px 0 30px;
}

.follow \* {
margin-right: 10px;
}

7. Links

/_ Links _/

.links {
background: #f2f2f2;
color: #616161;
font-size: 12px;
padding: 35px 0;
}

.links-inner {
max-width: 1100px;
margin: 0 auto;
padding: 0 20px;
display: grid;
grid-template-columns: repeat(6, 1fr);
grid-column-gap: 10px;
align-items: flex-start;
justify-content: center;
}

.links li {
line-height: 2.8;
}

    <!-- Links -->
    <section class="links">
      <div class="links-inner">
        <ul>
          <li><h3>What's New</h3></li>
          <li><a href="#">Surface Pro X</a></li>
          <li><a href="#">Surface Laptop 3</a></li>
          <li><a href="#">Surface Pro 7</a></li>
          <li><a href="#">Windows 10 apps</a></li>
          <li><a href="#">Office apps</a></li>
        </ul>
        <ul>
          <li><h3>Microsoft Store</h3></li>
          <li><a href="#">Account Profile</a></li>
          <li><a href="#">Download Center</a></li>
          <li><a href="#">Microsoft Store support</a></li>
          <li><a href="#">Returns</a></li>
          <li><a href="#">Older tracking</a></li>
        </ul>
        <ul>
          <li><h3>Education</h3></li>
          <li><a href="#">Microsfot in education</a></li>
          <li><a href="#">Office for students</a></li>
          <li><a href="#">Office 365 for schools</a></li>
          <li><a href="#">Deals for studentss</a></li>
          <li><a href="#">Microsfot Azure</a></li>
        </ul>
        <ul>
          <li><h3>Enterprise</h3></li>
          <li><a href="#">Azure</a></li>
          <li><a href="#">AppSource</a></li>
          <li><a href="#">Automotive</a></li>
          <li><a href="#">Government</a></li>
          <li><a href="#">Healthcare</a></li>
        </ul>
        <ul>
          <li><h3>Developer</h3></li>
          <li><a href="#">Visual Studio</a></li>
          <li><a href="#">Windowszs Dev Center</a></li>
          <li><a href="#">Developer Network</a></li>
          <li><a href="#">TechNet</a></li>
          <li><a href="#">Microsoft Developer</a></li>
        </ul>
        <ul>
          <li><h3>Company</h3></li>
          <li><a href="#">Careers</a></li>
          <li><a href="#">About Microsoft</a></li>
          <li><a href="#">Company news</a></li>
          <li><a href="#">Privacy at Microsoft</a></li>
          <li><a href="#">Inverstors</a></li>
        </ul>
      </div>
    </section>

8. Footer

/_ Footer _/

.footer {
background: #f2f2f2;
color: #616161;
font-size: 12px;
padding: 20px 0;
}

.footer-inner {
max-width: 1100px;
margin: 0 auto;
padding: 0 20px 0 20px;
display: flex;
align-items: center;
justify-content: space-between;
}

.footer div {
margin-bottom: 20px;
display: flex;
align-items: center;
}

.footer div i {
margin-right: 10px;
}

.footer ul {
display: flex;
flex-wrap: wrap;
}

.footer li {
margin-right: 30px;
margin-bottom: 20px;
}

    <!-- Footer -->
    <footer class="footer">
      <div class="footer-inner">
        <div><i class="fas fa-globe fa-2x"></i> English (United States)</div>
        <ul>
          <li><a href="#">Sitemap</a></li>
          <li><a href="#">Contact Microsoft</a></li>
          <li><a href="#">Privacy & cookies</a></li>
          <li><a href="#">Terms of use</a></li>
          <li><a href="#">Trademarks</a></li>
          <li><a href="#">Safety & eco</a></li>
          <li><a href="#">About our ads</a></li>
          <li><a href="#">&copy; Microsoft 2020</a></li>
        </ul>
      </div>
    </footer>
