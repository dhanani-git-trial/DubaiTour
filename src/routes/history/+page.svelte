<script>
  import Card from "$components/Card.svelte";
  import Nav from "$components/Nav.svelte";
  import "$css/history.css";
  // Select all .carousel-inner elements

    function trans() {
    const elements = document.querySelectorAll('.carousel-indicators');
    
    elements.forEach((element) => {
      element.style.transition = 'opacity 0.5s ease-in-out'; // Smooth transition for opacity
      element.style.opacity = 0; // Start fading out to 0

      // Listen for the transition end event
      element.addEventListener('transitionend', function onTransitionEnd() {
        // Once the opacity reaches 0, reverse the transition
        element.style.transition = 'opacity 0.5s ease-in-out'; // Ensure the transition is still smooth
        element.style.opacity = 1; // Fade back to 1

        // Remove the event listener to avoid repeating the logic
        element.removeEventListener('transitionend', onTransitionEnd);
      });
    });
  }

</script>



<Nav/>
<article>
<div class="carousel slide" data-ride="carousel" data-interval="1000000">
  <ol on:click={trans} class="carousel-indicators">
    <li data-target=".carousel" data-slide-to="0" class="active"></li>
    <li data-target=".carousel" data-slide-to="1"></li>
    <li data-target=".carousel" data-slide-to="2"></li>
    <li data-target=".carousel" data-slide-to="3"></li>
    <li data-target=".carousel" data-slide-to="4"></li>
    <li data-target=".carousel" data-slide-to="5"></li>
    <li data-target=".carousel" data-slide-to="6"></li>
    <li data-target=".carousel" data-slide-to="7"></li>
    <li data-target=".carousel" data-slide-to="8"></li>
    <li data-target=".carousel" data-slide-to="9"></li>
    <li data-target=".carousel" data-slide-to="10"></li>
  </ol>
  
  <div class="carousel-inner">
    <div class="carousel-item active">
      <Card>
        <span slot="title">1833: Establishment Of Dubai</span>
        <span slot="subtitle">The Al Maktoum family, led by Sheikh Maktoum bin Buti, took control of Dubai, marking the establishment of the Dubai Emirate. Dubai becomes a small fishing village and port town.</span>
      </Card>
    </div>
    <div class="carousel-item">
      <Card>
        <span slot="title">19th Century: Early Growth and Trade</span>
        <span slot="subtitle">Dubai grows as a trading hub. Its strategic location on the Persian Gulf attracts traders from India, Persia, and later, Europe. Pearling also becomes an important industry.</span>
      </Card>
    </div>
    <div class="carousel-item">
      <Card>
        <span slot="title">1900s: British Influence and Economic Development</span>
        <span slot="subtitle">In 1901, Dubai enters into a treaty with the British, and the British influence in the region grows, although Dubai remains largely independent. Then Dubai establishes itself as a key port for trading goods like textiles, pearls, and spices in 1930s.</span>
      </Card>
    </div>
    <div class="carousel-item">
      <Card>
        <span slot="title">1950s-1960s: Oil Discovery and Economic Shift</span>
        <span slot="subtitle">Oil exploration begins in the region. At this time, Dubai's economy is still largely dependent on trade and pearling. In 1966 Oil is discovered in Dubai, particularly in the Fateh oil field. Finally, in 1969, Dubai starts exporting oil, and the newfound wealth begins to transform the city.</span>
      </Card>
    </div>
    <div class="carousel-item">
      <Card>
        <span slot="title">1970s: Development of Infrastructure</span>
        <span slot="subtitle">Dubai becomes part of the United Arab Emirates (UAE), which was formed along with six other emirates. Then, in 1973, Dubai introduces its own currency, the UAE dirham, replacing the Gulf rupee. Moving into the Late 1970s, Dubai begins to invest heavily in infrastructure, including roads, buildings, and an airport. The city starts to transform into a modern metropolis.</span>
      </Card>
    </div>
    <div class="carousel-item">
      <Card>
        <span slot="title">1980s: Growth as a Financial Hub</span>
        <span slot="subtitle">In 1985, Dubai establishes the Dubai International Financial Centre (DIFC), beginning its rise as a global financial center. Then four years later Dubai drops its first shopping mall, the Al Ghurair Centre, opens in Dubai.</span>
      </Card>
    </div>
    <div class="carousel-item">
      <Card>
        <span slot="title">1990s: Urbanization and Tourism Boom</span>
        <span slot="subtitle">Dubai undergoes rapid urbanization, with iconic buildings such as the Burj Al Arab, an iconic luxury hotel, being built. The city's tourism industry also begins to grow. Then, one year before the 2000's finally turn corner in 1999, the opening of the Dubai Internet City marks a move to become a global tech hub.</span>
      </Card>
    </div>
    <div class="carousel-item">
      <Card>
        <span slot="title">2000s: Modernization and Global Recognition</span>
        <span slot="subtitle">The year 2000 finally comes, Dubai announces plans for large-scale projects, including artificial islands like Palm Jumeirah and luxury resorts. 2004, Dubai Ports World (DP World) is established and expands globally, cementing Dubai as a major shipping hub. Years 2008 and 2009, The global financial crisis temporarily hits Dubai, but it recovers quickly with strong leadership and economic diversification.</span>
      </Card>
    </div>
    <div class="carousel-item">
      <Card>
        <span slot="title">2010s: Becoming a Global Destination</span>
        <span slot="subtitle">In the year 2010, The Burj Khalifa, the world’s tallest building, is completed and becomes a symbol of Dubai’s ambitions and success. In that same year, Dubai also builds The Palm Jumeirah, an artificial island shaped like a palm tree, which becomes a major landmark in Dubai's skyline. 2012, The Dubai Mall, one of the largest shopping malls in the world, opens. The year 2014, Dubai wins the bid to host the 2020 World Expo (which was postponed 2021 due to the pandemic). 2015: Dubai International Airport becomes the busiest airport in the world for international passengers. The Next year, 2022, Dubai continues to expand its global business presence, with the UAE becoming a leader in renewable energy, technology, and tourism. Pushing towards 2023, Dubai continues to invest in futuristic infrastructure, with projects like the Museum of the Future and the development of autonomous transportation systems.</span>
      </Card>
    </div>
    <div class="carousel-item">
      <Card>
        <span slot="title">2020s: Post-Pandemic Recovery and Innovation</span>
        <span slot="subtitle">In the year 2021 after the COVID-19 pandemic, The Expo 2020 finally Dubai opens, showcasing global innovations in sustainability, mobility, and opportunity (delayed due to COVID-19).</span>
      </Card>
    </div>
    <div class="carousel-item">
      <Card>
        <span slot="title">2025: Building The New Future</span>
        <span slot="subtitle">Moving into 2025, Dubai is positioning itself to be a leader in sectors such as artificial intelligence, smart cities, and space exploration. Now, Dubai is expected to continue its trend of economic diversification, with significant advancements in technology, sustainability, and cultural development. The city aims to be a global leader in areas like smart cities, artificial intelligence, and space exploration.</span>
      </Card>
    </div>
  </div>
  
  <!-- Navigation buttons -->
  <button on:click={trans} class="carousel-control-prev" style="opacity: 1;" href=".carousel" data-slide="prev">
    <span class="carousel-control-prev-icon" aria-hidden="true"></span>
    <span class="sr-only">Previous</span>
  </button>
  <button on:click={trans} class="carousel-control-next" style="opacity: 1;" href=".carousel" data-slide="next">
    <span class="carousel-control-next-icon" aria-hidden="true"></span>
    <span class="sr-only">Next</span>
  </button>
</div>
</article>
