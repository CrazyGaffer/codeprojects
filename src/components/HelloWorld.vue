<template>
  <form action="http://localhost:8888" method="post">
    <div class="container">
      <h2>Please enter your name and pick the sector</h2>
      <label>
        <b>Username</b>
      </label>
      <input type="text" placeholder="Enter your name" name="uname" required>
      <label>
        <b>Sectors</b>
      </label>

     <input type="search" placeholder="Select sector" name="sectors_select" list="sectors" required>
      <datalist id="sectors">
        <option value="Contractions Materials">Manufacturing</option>
        <option value="Products">Bakery & confectionery products</option>
        <option value="Electronics and Optics">Manufacturing</option>
        <option value="Beverages">Products</option>
        <option value="Fish and fish products">Products</option>
        <option value="Meat and meat products">Products</option>
        <option value="Milk and dairy products">Products</option>
        <option value="Bathroom/sauna">Furniture</option>
        <option value="Bedroom">Furniture</option>
        <option value="Children's">Furniture</option>
        <option value="Kitchen">Furniture</option>
      </datalist>
        <br><br>
      <button type="submit">Save</button>
      <label>
        <input type="checkbox" name="remember" required> Agree to Terms
      </label>
    </div>

  </form>
</template>

<script>


export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
}


</script>


<style scoped>
body {
  text-align: center;
}

form {
  border: 3px solid #f1f1f1;
  margin: 0 auto;
  width: 50%;
}


input[type=text],[type=search] {
  width: 100%;
  padding: 12px 20px;
  margin: 8px 0;
  display: inline-block;
  border: 1px solid #ccc;
  box-sizing: border-box;
}

button {
  background-color: #046aaa;
  color: white;
  padding: 14px 20px;
  margin: 8px 0;
  border: none;
  cursor: pointer;
  width: 100%;
}

button:hover {
  opacity: 0.8;
}

.container {
  padding: 16px;
}


@media screen and (max-width: 300px) {

}
</style>
