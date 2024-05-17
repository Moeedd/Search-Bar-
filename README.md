<?php get_header();
// Template Name: Test
?>
<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css">
<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min.js"></script>
<style>
  @media(min-width: 1200px){
        .elementor-container, .container{
        max-width: 1280px !important;
    }
  }
  form{
      font-family: poppins;
  }
  div#search-results {
    padding-top: 50px;
    padding-bottom: 40px;
}

.box a:hover{
    text-decoration: none !important;
}
.btn-main a:hover{
    text-decoration: none !important;
}
.btn-main a {
    text-align: center;
    font-family: &#039;
    font-size: 14px;
    font-weight: 600;
    color: white;
    background-color: #0E2E5B;
    padding: 5px 5px 5px 5px;
    border-radius: 5px;
    font-family: poppins;
    margin: 10px 0px 0px 0px;
}
  .row>* {
    display: inline-block;
    vertical-align: top;
    /* Align items to the top */
    margin-right: 10px;
    /* Add some space between items */
  }

  .row {
    display: flex;
    flex-direction: row;
    justify-content: center;
    flex-wrap: nowrap;
  }
  .content-row p{
      font-family: poppins;
  }
  #search-results > .row>* {

    padding: 0px;
}
div#search-results .content h2 {
    font-family: poppins;
    font-size: 22px;
    font-weight: 600;
    margin: 10px 0px;
}
div#search-results > .row {
    display: flex;
    flex-direction: row;
    justify-content: unset;
    flex-wrap: wrap;
  }
  div#search-results > .row > .col-md-3 {
    margin-right: unset !important;
    padding: 0 5px;
  }
  .e-h1-t {

    margin-left: -27px;
}
button.dealer-fp-searchbar-button.form-control {
    color: #0E2E5B;
    font-weight: 700;
    transition: all .2s ease;
}
button.dealer-fp-searchbar-button.form-control:hover {
    color: white;
    font-weight: 700;
    background-color: #0E2E5B;
}
select.form-control {
    background-position: calc(100% - 13px) 13px !important;
    background-image: url(https://www.carolinadirecthomes.com/wp-content/uploads/2024/04/8541675_caret_down_icon.png) !important;
}
@media(max-width: 1199px) and (min-width: 768px){
  div#search-results > .row {
    flex-wrap: wrap !important;
    display: flex !important;
    justify-content: space-between;
}
div#search-results .row .col-md-3 {
    flex: 0 0 48% !important;
    max-width: 48%;
}
.e-h1-t {
    margin-left: 0px;
}
.dealer-fp-searchbar {
    margin: 0 auto;
    padding: 20px 20px 30px 20px;
}
.form-cont .col-md-12 {
    flex: 0 0 50%;
    margin: 10px 0px 0px 0px;
}
#floorplan-searchbar .row{
    flex-wrap: wrap !important;
}
}
@media(max-width: 767px){
    .btn-cont .row .col-md-6 {
    flex: 0 0 46%;
}
div#search-results {
    padding-top: 30px;
    padding-bottom: 20px;
    padding-left: 40px;
    padding-right: 40px;
}
.btn-cont .row {
    display: flex;
    flex-wrap: wrap;
}
div#search-results > .row {
    flex-wrap: wrap;
}
.form-cont .row {
    flex-wrap: wrap;
}
.dealer-fp-searchbar {
    margin: 0 auto;
    padding: 20px 20px 30px 20px;
}
form#floorplan-searchbar .col-md-12 {
    flex: 0 0 50%;
    padding: 10px 10px 0px 0px;
    margin: 0px;
}
form#floorplan-searchbar select, form#floorplan-searchbar button {
    font-size: 13px !important;
}
.e-h1-t {
    margin-left: -15px;
}

}
</style>
<div class="elementor-inventory-banner">
    <?php 
     $elementor_shortcode = '[elementor-template id="4475"]'; // Replace with your Elementor template shortcode
    echo do_shortcode($elementor_shortcode);
    
    ?>
</div>
<div class="form-cont">
    <div class="container">
    <form method="POST" class="dealer-fp-searchbar" id="floorplan-searchbar">
    <h3 class="e-h1-t">Search Floor Plans</h3>
    <div class="row">
        <div class="col-lg-2 col-md-12">
            <select name="home_type" class="form-control">
                <option class="option" selected="selected" value="">Manufacturer</option>
                <option class="option" value="feetwood_home">Fleetwood Homes</option>
                <option class="option" value="legacy_homes">Legacy Homes</option>
                <option class="option" value="champion-homes">Champion Homes</option>
            </select>
        </div>
        <div class="col-lg-2 col-md-12 series">
            <select name="category" class="form-control">
                <option class="option" selected="selected" value="">Series</option>
                <optgroup label="Fleetwood Homes">
                    <option class="option" value="edge">Edge</option>
                    <option class="option" value="xtreme">Xtreme</option>
                </optgroup>
                <!-- Add other optgroup elements as needed -->
            </select>
        </div>
        <div class="col-lg-2 col-md-12">
         <select name="square_feet" class="form-control">
                <option class="option" selected="selected" value="">Sq Ft</option>
                <option class="option" value="100-500">100-500</option>
                <option class="option" value="500-1000">500-1000</option>
                <option class="option" value="1000-1500">1000-1500</option>
                <option class="option" value="1500-2000">1500-2000</option>
                <option class="option" value="2000">2000+</option>
            </select>
        </div>
        <div class="col-lg-2 col-md-12">
            <select name="bedrooms" class="form-control">
                <option selected="selected" value="">Beds</option>
                <option value="1">1</option>
                <option value="2">2</option>
                <option value="3">3</option>
                <option value="4">4</option>
                <option value="5">5</option>
            </select>
        </div>
        <div class="col-lg-2 col-md-12">
            <select name="bathrooms" class="form-control">
                <option selected="selected" value="">Baths</option>
                <option value="1">1</option>
                <option value="2">2</option>
                <option value="3">3</option>
                <option value="4">4</option>
            </select>
        </div>
        <div class="col-lg-2 col-md-12">
            <button type="submit" class="dealer-fp-searchbar-button form-control">Search</button>
        </div>
    </div>
</form>

</div>
</div>

<div class="container" id="search-results">
    <div class="row">
        <?php
          $args = array(
        'post_type' => 'my_inventory', // Change 'my_inventory' to your custom post type
        'posts_per_page' => -1,
        );
        // Check if form data is submitted
        if ($_SERVER["REQUEST_METHOD"] == "POST") {
            $home_type = sanitize_text_field($_POST['home_type']);
            $category = sanitize_text_field($_POST['category']);
            $beds = sanitize_text_field($_POST['bedrooms']);
            $baths = sanitize_text_field($_POST['bathrooms']);
            $sqft = sanitize_text_field($_POST['square_feet']);
            
            // WP_Query arguments to filter floor plans based on form data
          $args = array(
                'post_type' => 'my_inventory', // Change 'my_inventory' to your custom post type
                'posts_per_page' => -1, // Retrieve all posts, you can adjust the number as needed
                'post_status' => 'publish', // Retrieve only published posts
                'tax_query' => array(
                    'relation' => 'AND', // Filter with AND relation
                ),
            );

            // Check and add tax_query conditions based on the provided form inputs
            if (!empty($home_type)) {
                $args['tax_query'][] = array(
                    'taxonomy' => 'home_type', // Change 'home_type' to your taxonomy name
                    'field' => 'slug',
                    'terms' => $home_type,
                );
            }
            if (!empty($category)) {
                $args['tax_query'][] = array(
                    'taxonomy' => 'category', // Change 'category' to your taxonomy name
                    'field' => 'slug',
                    'terms' => $category,
                );
            }
            if (!empty($beds)) {
                $args['tax_query'][] = array(
                    'taxonomy' => 'bedrooms', // Change 'bedrooms' to your taxonomy name
                    'field' => 'slug',
                    'terms' => $beds,
                );
            }
            if (!empty($baths)) {
                $args['tax_query'][] = array(
                    'taxonomy' => 'bathrooms', // Change 'bathrooms' to your taxonomy name
                    'field' => 'slug',
                    'terms' => $baths,
                );
            }
      if (!empty($sqft)) {
    if (strpos($sqft, '-') !== false) {
        // If it's a range, split the string to get the minimum and maximum values
        list($min_sqft, $max_sqft) = explode('-', $sqft);

        // Add meta query to filter posts within the range
        $args['meta_query'][] = array(
            'key'     => 'square_feet', // Replace with your ACF field name
            'value'   => array($min_sqft, $max_sqft),
            'type'    => 'NUMERIC',
            'compare' => 'BETWEEN',
        );
    } elseif ($sqft === '2000') {
        // If the selected square footage is "2000+", filter posts with square footage greater than or equal to 2000
        $args['meta_query'][] = array(
            'key'     => 'square_feet', // Replace with your ACF field name
            'value'   => $sqft,
            'type'    => 'NUMERIC',
            'compare' => '>=', // Greater than or equal to
        );
    }
}
        
        

}
       
        // The Query
        $query = new WP_Query($args);

        // The Loop
        if ($query->have_posts()) {
            while ($query->have_posts()) {
                $query->the_post(); ?>
                <div class="col-md-3">
                    <div class="box">
                        <a href="<?php the_permalink(); ?>">
                            <?php if (has_post_thumbnail()) : ?>
                                <div class="thumbnail">
                                    <?php the_post_thumbnail('medium', ['class' => 'img-fluid']); ?>
                                </div>
                            <?php endif; ?>
                            <div class="content">
                                <h2><?php the_title(); ?></h2>
                                <div class="content-row">
                                              <?php
                                // Retrieve the taxonomy terms for the post
                                $beds = get_the_terms(get_the_ID(), 'bedrooms');
                                $sq_ft = get_the_terms(get_the_ID(), 'square_feet');
                                $baths = get_the_terms(get_the_ID(), 'bathrooms');
            
                                // Display the taxonomy terms
                                if ($beds) {
                                    echo '<p><b>Beds:</b> ' . $beds[0]->name . '</p>';
                                }
                                if ($sq_ft) {
                                    echo '<p><b>Sq ft:</b> ' . $sq_ft[0]->name . ' </p>';
                                }
                                if ($baths) {
                                    echo '<p><b>Baths:</b> ' . $baths[0]->name . ' </p>';
                                }
                                ?>
                                </div>
                      
                            </div>
                            <div class="btn-cont">
                                <div class="row">
                                    <div class="col-md-6">
                                        <div class="btn-main">
                                            <a href="<?php the_permalink(); ?>">Learn More</a>
                                        </div>
                                    </div>
                                      <div class="col-md-6">
                                        <div class="btn-main">
                                             <a href="https://www.carolinadirecthomes.com/contact-us/">Get Quote</a>
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </a>
                    </div>
                </div>
        <?php
            }

            // Restore original Post Data
            wp_reset_postdata();
        }
        ?>
    </div>
</div>
</div>
</div>
</div>
<div class="elementor-slider-main">
    <?php 
     $elementor_shortcode = '[elementor-template id="4472"]'; // Replace with your Elementor template shortcode
    echo do_shortcode($elementor_shortcode);
    
    ?>
</div>

<script>
$(document).ready(function(){
    // AJAX form submission
    $('#floorplan-searchbar').submit(function(e){
        e.preventDefault(); // Prevent default form submission
        var formData = $(this).serialize(); // Serialize form data

        // AJAX request
        $.ajax({
            type: 'POST',
            url: window.location.href, // PHP script to handle form submission and filter results
            data: formData,
            success: function(response){
                console.log(formData)
                    var doc = document.createElement('div');
                    doc.innerHTML = response;
                    var extractedSection = doc.querySelector('#search-results');
                    if (extractedSection !== null) {
                               $('#search-results').html(extractedSection.innerHTML);
                               console.log(extractedSection.innerHTML);
                    } else {
                        console.error('Specified section not found in the response.');
                    }
            }
        });
    });
});
</script>

<?php get_footer();?>
