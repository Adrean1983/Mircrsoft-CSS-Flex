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
