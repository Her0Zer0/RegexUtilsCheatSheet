_Longitude Example_

```.js
var long_pattern=/^(\+|-)?(?:180(?:(?:\.0{1,6})?)|(?:[0-9]|[1-9][0-9]|1[0-7][0-9])(?:(?:\.[0-9]{1,6})?))$/;
var test_longitude=[
    "90",
    "-90.01",
    "90.01123",
    "86",
    "180.01",
    "180.000",
    "-180.001",
    "-181.0"
];

test_longitude.forEach((long)=>{
    console.log(`${long} matched: ${long.match(long_pattern) != null}`);
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

