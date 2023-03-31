# WeatherApp
A weather website is a website that provides users with information about current and forecasted weather conditions for a specific location.


'''HTML

<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Weather App</title> <!-- titel of the webpage-->
  <link rel="preconnect" href="https://fonts.gstatic.com">
  <link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Open+Sans&display=swap" rel="stylesheet">
  <link rel="stylesheet" href="./sytle.css"> <!-- Adding Css in Html -->
  <script src="./script.js" defer></script> <!--Adding Js in Html-->
</head>
<!---->
<body>
  <div class="card">
    <div class="search">
      <input type="text" class="search-bar" placeholder="Search">
      <button><svg stroke="currentColor" fill="none" stroke-width="2" viewBox="0 0 24 24" stroke-linecap="round" stroke-linejoin="round" height="1.5em" width="1.5em" xmlns="http://www.w3.org/2000/svg"><circle cx="11" cy="11" r="8"></circle><line x1="21" y1="21" x2="16.65" y2="16.65"></line></svg></button>
    </div>
    <div class="weather loading">
      <h2 class="city">Weather in Delhi</h2>
      <h1 class="temp">33°C</h1>
      <div class="flex">
        <img src="https://openweathermap.org/img/wn/04n.png" alt="" class="icon" /> <!--Adding image for the icon-->
        <div class="description">Sunny</div>
      </div>
      <div class="humidity">Humidity: 60%</div>
      <div class="wind">Wind speed: 6.2 km/h</div>
    </div>
  </div>
</body>

</html>'''






''' CSS

body {
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
    margin: 0;
    font-family: 'Open Sans', sans-serif;    background: #222;
    background-image: url('https://source.unsplash.com/1600x900/?landscape');/* background image */
    font-size: 120%;
  }
  
  .card {  /* to create a styled container element that is used to display content */
    background: #000000d0;
    color: white;
    padding: 2em;
    border-radius: 50px;
    width: 100%;
    max-width: 420px;
    margin: 2em;
  }
  
  .search {
    display: flex;
    align-items: center; /* Used to aligning item to the center */
    justify-content: center;
  }
  
  button { /* In this part desiging the search button*/
    margin: 0.5em;
    border-radius: 50%;
    border: none;
    height: 44px;
    width: 44px;
    outline: none;
    background: #7c7c7c2b;
    color: white;
    cursor: pointer;
    transition: 0.2s ease-in-out;
  }
  /**/
  input.search-bar { /* In this part Designing the Search bar */
    border: none;
    outline: none;
    padding: 0.4em 1em;
    border-radius: 24px; /* to define rounded corners for the  border*/
    background: #7c7c7c2b;  /*Background color for the search bar */
    color: white; /* Color for the text that are written on the search bar  */
    font-family: inherit; /* Defining the font style on the search bar */
    font-size: 105%;
    width: calc(100% - 100px);
  }
   
  button:hover {     /* Set the background color for the search bar */
    background: #7c7c7c6b;
  }
  
  h1.temp {
    margin: 0;
    margin-bottom: 0.4em;
  }
  
  .flex {
    display: flex;
    align-items: center;
  }
  
  .description {
    text-transform: capitalize;
    margin-left: 8px;
  }
  
  /* .weather.loading {
    visibility: hidden;
    max-height: 20px;
    position: relative;
  }
  
  .weather.loading:after {
    visibility: visible;
    content: "Loading...";
    color: white;
    position: absolute;
    top: 0;
    left: 20px;
  } */ '''
