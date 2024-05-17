# Search-Bar-
Php Search Bar Custom post type ui
<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Document</title>
</head>
<style>
    .search-form {
    margin-bottom: 2rem;
  }
  
  .search-form form {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    align-items: center;
  }
  
  .search-form label {
    display: block;
    margin-bottom: 0.5rem;
    font-weight: bold;
  }
  
  .search-form select {
    margin-bottom: 1rem;
    padding: 0.5rem;
    border: 1px solid #ccc;
    border-radius: 4px;
    width: 100%;
    box-sizing: border-box;
  }
  
  .search-form input[type="submit"] {
    padding: 0.5rem 1rem;
    border: none;
    border-radius: 4px;
    background-color: #4CAF50;
    color: white;
    cursor: pointer;
  }
  
  .search-form input[type="submit"]:hover {
    background-color: #3e8e41;
  }
  
  .search-form a {
    padding: 0.5rem 1rem;
    border: none;
    border-radius: 4px;
    background-color: #333;
    color: white;
    text-decoration: none;
    cursor: pointer;
  }
  
  .search-form a:hover {
    background-color: #222;
  }

</style>

<body>
  <section class="search-form">
    <form id="search-form">
      <label for="manufacturer">Manufacturer:</label>
      <select id="manufacturer" name="manufacturer">
        <option value="any">Manufacturer</option>
        <option value="Fleetwood Homes">Fleetwood Homes</option>
        <option value="Legacy Homes">Legacy Homes</option>
        <option value="Champion Homes">Champion Homes</option>
      </select>

      <label for="series">Series:</label>
      <select id="series" name="series">
        <option value="any">Series</option>
        <option value="Eddge">Eddge</option>
        <option value="Xtreme">Xtreme</option>
      </select>

      <label for="sqft">Sq Ft:</label>
      <select id="sqft" name="sqft">
        <option value="any">Sq Ft</option>
        <option value="1000">1000 sq ft</option>
        <option value="2000">2000 sq ft</option>
      </select>

      <label for="beds">Beds:</label>
      <select id="beds" name="beds">
        <option value="any">Beds</option>
        <option value="1">1 bed</option>
        <option value="2">2 beds</option>
      </select>

      <label for="baths">Baths:</label>
      <select id="baths" name="baths">
        <option value="any">Baths</option>
        <option value="1">1 bath</option>
        <option value="2">2 baths</option>
      </select>

      <input type="submit" value="SEARCH">
    </form>
  </section>
  <section id="home-details" style="display: none;">
    <h2>Home Details</h2>
    <div id="home-image">
      <!-- Placeholder for home image -->
      <img src="home-image-placeholder.jpg" alt="Home Image">
    </div>
    <div id="home-description">
      <!-- Placeholder for home description -->
      <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nullam lacinia libero vel enim tincidunt, ac gravida eros condimentum. Duis efficitur mauris sit amet semper gravida.</p>
    </div>
  </section>

  <script>
    document.getElementById('search-form').addEventListener('submit', function(event) {
      event.preventDefault(); // Prevent form submission

      // Get selected values from form fields
      var manufacturer = document.getElementById('manufacturer').value;
      var series = document.getElementById('series').value;
      var sqft = document.getElementById('sqft').value;
      var beds = document.getElementById('beds').value;
      var baths = document.getElementById('baths').value;

      // Display home details section
      var homeDetailsSection = document.getElementById('home-details');
      homeDetailsSection.style.display = 'block';

      // Update home image and description (replace placeholders with actual values)
      var homeImage = document.getElementById('home-image');
      homeImage.innerHTML = '<img src="path-to-home-image.jpg" alt="Home Image">';

      var homeDescription = document.getElementById('home-description');
      homeDescription.innerHTML = '<p>Description of the home goes here.</p>';
    });
  </script>

  
</body>

</html>
