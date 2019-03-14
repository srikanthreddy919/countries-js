# countries-js

A JavaScript library to populate country &amp; state dropdown lists containing all the country names and state names.

# usage

You can call countries js in two ways

#### 1. Using HTML data attributes

html markup for data-attributes

```
<div data-toggle-group="location">
  <div class="form-group">
    <label>Country</label>
    <select class="form-control" name="country" data-toggle="country" data-country=""></select>
  </div>
  <div class="form-group">
    <label>State</label>
    <select class="form-control" name="country" data-toggle="state" data-state=""></select>
  </div>
</div>

```

and call `loadCountries()` function on `Document` load

```
<script type="text/javascript">
  document.addEventListener("load", loadCountries());
</script>

```
to populate selected values use below `data attributes`

for country `data-country=countryName` 

for state `data-state=stateName`

#### 2. Using javascript

you can call `populateCountries()` function with `countryElement` and `stateElement` parameters

First find the `elements` and pass as parameters as shown below

```
<script type="text/javascript">
  var country_element = document.getElementById('#country);
  var state_element = document.getElementById('#state);
  document.addEventListener("load", populateCountries(country_element, state_element));
</script>

```

You can find the `index.html` for reference.

# Thank you
