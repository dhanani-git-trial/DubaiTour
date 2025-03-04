<script>
  import '$css/nav.css';
  import Logo from '$lib/images/logo.png';
</script>


<header>
  <div class="navbar">
      <div class="logo">
          
      </div>
      <div class="nav">
          <ul>
            <img src={Logo} alt="Dubai"/>
              <li><a href="#">About</a></li>
              <li><a href="#">Projects</a></li>
              <li><a href="#">Skills</a></li>
              <li><a href="#">Blog</a></li>
              <li><a href="#">Contact</a></li>
          </ul>
          <div class="menu"><i class="fa-solid fa-bars"></i></div>
      </div>
      <a href="#" class="highlight">Download CV</a>
      <div class="dropdown-menu">
          <ul>
              <li><a href="#">About</a></li>
              <li><a href="#">Projects</a></li>
              <li><a href="#">Skills</a></li>
              <li><a href="#">Blog</a></li>
              <li><a href="#">Contact</a></li>
              <li><a href="#" class="highlight">Download CV</a></li>
          </ul>
      </div>
  </div>
</header>