<script>
  import Nav from "$components/Nav.svelte";
  import Card from "$components/Card.svelte";
  import "$css/form.css";
  import Footer from "$components/Footer.svelte";
</script>

<Nav />
<br /><br /><br />
<Card>
  <span slot="title">
    <form>
      <script>
        function addToLocalStorage(section, value) {
          let data = JSON.parse(localStorage.getItem("userSelections")) || {};
          if (!data[section]) data[section] = [];
          data[section].push(value);
          localStorage.setItem("userSelections", JSON.stringify(data));
        }

        function handleAdd(sectionId, sectionName) {
          const value = document.getElementById(sectionId).value;
          if (sectionId === "transportation") {
            const from = document.getElementById("transportationFrom").value;
            const to = document.getElementById("transportationTo").value;
            const combinedValue = `${value} (From: ${from} - To: ${to})`;
            addToLocalStorage(sectionName, combinedValue);
            alert(`${combinedValue} added to ${sectionName}`);
          } else {
            addToLocalStorage(sectionName, value);
            alert(`${value} added to ${sectionName}`);
          }
        }
      </script>

      <!-- Transportation Section -->
      <div class="form-group">
        <label for="transportation">Transportation - $2</label>
        <select class="form-control" id="transportation">
          <option>Taxi</option>
          <option>Bus</option>
          <option>Train</option>
          <option>Rental Car</option>
        </select>

        <label for="transportationFrom" class="mt-2">From</label>
        <input
          type="text"
          class="form-control"
          id="transportationFrom"
          placeholder="Starting Location"
        />

        <label for="transportationTo" class="mt-2">To</label>
        <input
          type="text"
          class="form-control"
          id="transportationTo"
          placeholder="Destination"
        />

        <div class="text-end mt-2">
          <button
            type="button"
            class="btn btn-info"
            on:click={() => handleAdd("transportation", "Transportation")}
          >
            Add Transportation
          </button>
        </div>
      </div>

      <!-- Places Discount Section -->
      <div class="form-group">
        <label for="placesDiscount">Additional Places Discount</label>
        <select class="form-control" id="placesDiscount">
          <option>Burj Khalifa - $15 USD discount</option>
          <option>Desert Safari - $15 USD discount</option>
          <option>Aquaventure Waterpark - $10 USD discount</option>
        </select>
        <div class="text-end">
          <button
            type="button"
            class="btn btn-info mt-2"
            on:click={() => handleAdd("placesDiscount", "Places Discount")}
          >
            Add
          </button>
        </div>
      </div>

      <!-- Food Options Section -->
      <div class="form-group">
        <label for="foodOptions">Food Discount</label>
        <select class="form-control" id="foodOptions">
          <option>Palm Jumeriah Cafe - $3 USD discount</option>
          <option>24th St. World Street Food Dubai - $5 USD discount</option>
          <option>Halal</option>
          <option>Gluten-Free</option>
        </select>
        <div class="text-end">
          <button
            type="button"
            class="btn btn-info mt-2"
            on:click={() => handleAdd('foodOptions', 'Food Options')}
          >
            Add
          </button>
        </div>
      </div>

      <div class="text-center mt-4">
        <button
  type="button"
  class="btn btn-success"
  on:click={() => window.location.href = 'https://dhanani-git-trial.github.io/DubaiTour/confirm/'}
>
  My Discounts
</button>
      </div>
    </form>
  </span>
</Card>
<Footer />
