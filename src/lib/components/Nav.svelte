<script>
  import '$css/global.css';
  import Logo from '$lib/images/logo.png';
  import { base } from '$app/paths';
</script>


<nav>
  <div class="navbar">
      <div class="nav">
          <ul>
            <img src={Logo} alt="Dubai"/>
              <li><a href="{base}/">About</a></li>
              <li><a href="{base}/history">History</a></li>
              <li><a href="{base}/attractions">Attractions</a></li>
              <li><a href="#">Blog</a></li>
              <li><a href="#">Contact</a></li>
          </ul>
          <div class="menu"><i class="fa-solid fa-bars"></i></div>
      </div>
  </div>
</nav>