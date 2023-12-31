# js-countries-states-cities
A simple javascript library using json files to populate the data for countries, states and cities.

## Insights
Total Regions : 6
Total Sub Regions : 22
Total Countries : 250
Total States/Regions/Municipalities : 5,081
Total Cities/Towns/Districts : 150,540

## How to install

```bash
    npm i js-countries-states-cities
```

## How to use

```js
    // Latest version - v1.0.0
    let { Country, State, City } = require('js-countries-states-cities');

    // available methods for Country 
    console.log(Country.getList());
    console.log(Country.getById(1));
    console.log(Country.search('Pakistan'));
    console.log(Country.getByIdWithStates(167));
    console.log(Country.getByIdWithCities(167));

    // available methods for State
    console.log(State.getList());
    console.log(State.getById(1));
    console.log(State.getByIdWithCities(3176));
    console.log(State.search({ search: "punjab", country: 167 })); //country is optional
    console.log(State.search("punjab"));

    // available methods for City
    console.log(City.getList());
    console.log(City.getById(1));
    console.log(City.search({ search: "lahore", state: 3176, country: 167 })); //country, state is optional
    console.log(City.search("lahore"));


```
