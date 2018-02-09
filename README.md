# country-region-city-api

An API developed by [MedUnes](https://medunes.net). 
World country + world regions + world cities in dependent dropdown menus.
Very suitable for sign up forms, shipping forms, etc. 

API Key can be obtained from [here](https://battuta.medunes.net).

Original Demo is provided by [MedUnes](https://codepen.io/medunes/pen/GWoojz), but it depends on multiple factors such 'Materialize css and js'. I also found that it doesn't fully support mobile and tablets platforms. Also, the dropdown arrows seem to be duplicated. 

# My demos by versions
1. [V1.0](https://codepen.io/sam-shudukhi/full/EQNMvy)
2. [V2.0](https://codepen.io/sam-shudukhi/full/oEZeJP).

# Temporary API key provided by MedUnes (will be unavailable soon): 
```
var key = '00000000000000000000000000000000';
```

# My obtained API key for testing purposes. I advise you to obtain your own from [here](https://battuta.medunes.net).
```
var key = 'e2425c439df5e00f3e803ceaf4f6512c';
```
# Versions:
* V1.0 --> Feb 7th, 2018.
* V2.0 --> Feb 9th, 2018.

- Latest Update:
1. Design is slightly improved and updated, but kept the simple look for ease modifications by users.
2. Put together in an HTML form along with a username and password fields to get a form look and style.
3. Country select field uses country codes in the value attribute of an option. In V2.0, country code was moved to the id attribute of the option and the country name was put in the value attribute for easier data collection.

```
$("#country").append(
        '<option id="'+ value.code +'" value="' + value.name + '">' + value.name + "</option>"
      );
$("#country").change(function() {
    countryCode = $(this).children(":selected").attr("id");
    });
```

# Requirement:
- Bootstrap.
```
<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css">

```
jQuery.
```
<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.2.1/jquery.min.js"></script>
```
# Sam-Shudukhi 
