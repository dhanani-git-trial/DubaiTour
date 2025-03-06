<script>
    import Nav from '$components/Nav.svelte';
    import Card from '$components/Card.svelte';
    import '$css/form.css';
</script>
<Nav/>
<br><br><br>
<Card>
<span slot="title">
  
<form>
  <div class="form-group">
    <label for="formGroupExampleInput">First Name</label>
    <input type="text" class="form-control" id="formGroupExampleInput" placeholder="First Name">
  </div>
    <div class="form-group">
    <label for="formGroupExampleInput">Last Name</label>
    <input type="text" class="form-control" id="formGroupExampleInput" placeholder="Last Name">
  </div>
  <div class="form-group">
    <label for="exampleFormControlInput1">Email address</label>
    <input type="email" class="form-control" id="exampleFormControlInput1" placeholder="Email Adress">
  </div>
  <div class="form-group">
    <label for="exampleFormControlSelect1">Example select</label>
    <select class="form-control" id="exampleFormControlSelect1">
      <option>1</option>
      <option>2</option>
      <option>3</option>
      <option>4</option>
      <option>5</option>
    </select>
  </div>
  <div class="form-group">
    <label for="exampleFormControlSelect2">Select amount of people</label>
    <select multiple class="form-control" id="exampleFormControlSelect2">
      <option>1</option>
      <option>2</option>
      <option>3</option>
      <option>4</option>
      <option>5</option>
      <option>2</option>
      <option>3</option>
      <option>4</option>
      <option>5</option>
    </select>
  </div>
  <div class="form-group">
    <label for="exampleFormControlTextarea1">Example textarea</label>
    <textarea class="form-control" id="exampleFormControlTextarea1" rows="3"></textarea>
  </div>
  <iframe src="form.html"></iframe>
  <div class="text-center"><button type="button" class="btn btn-success">Submit</button></div>
</form>
</span>

</Card>
