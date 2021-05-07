_Mac Address Example_

```.js
/**
 * 
 *  Matches these
 *  a1:b2:c3:d4:e5:f6
 *  fe-0E-ab-10-0d-EE
 * 
 *  Doesn't match these
 *  a1.b2.c3.d4.e5.f6
 *  a1|b2|c3|d4|e5|f6
 * 
 */

var mac_address_pattern=/^([0-9A-Fa-f]{2}[:-]){5}([0-9A-Fa-f]{2})$/gm;
var test_mac_addresses=[
    "a1:b2:c3:d4:e5:f6",
    "fe-0E-ab-10-0d-EE",
    "a1.b2.c3.d4.e5.f6",
    "a1|b2|c3|d4|e5|f6"
];

test_mac_addresses.forEach((mac)=>{
    console.log(`${mac} matched: ${mac.match(mac_address_pattern) != null}`);
});
```
