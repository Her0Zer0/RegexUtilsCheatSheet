_Latitude Example_

```.js
var lat_pattern=/^(\+|-)?(?:90(?:(?:\.0{1,6})?)|(?:[0-9]|[1-8][0-9])(?:(?:\.[0-9]{1,6})?))$/;
var test_latitude=[
    "90",
    "-90.01",
    "90.01123",
    "86",
    "47.2521",
    "180.01",
    "180.000",
    "-180.001",
    "-181.0"
];

test_latitude.forEach((lat)=>{
    console.log(`${lat} matched: ${lat.match(lat_pattern) != null}`);
});

// 90 matched: true
// -90.01 matched: false
// 90.01123 matched: false
// 86 matched: true
// 47.2521 matched: true
// 180.01 matched: false
// 180.000 matched: false
// -180.001 matched: false
// -181.0 matched: false

```
