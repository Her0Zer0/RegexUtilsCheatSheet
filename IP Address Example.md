_Ip Address Example_

```.js

/**
 *  Matches these 
 *  172.168.10.28
 *  172.18.1.233
 *  10.168.10.28
 *  8.8.0.8
 * 
 */

var ip_pattern=/\b(?:\d{1,3}\.){3}\d{1,3}\b/gm; 

var test_ip_addresses=[
    "172.168.10.28",
    "192.18.1.233",
    "10.168.10.28",
    "8.8.0.8", 
    "172:168:10:28",
    "172|168|10|28",
];

test_ip_addresses.forEach((ip)=>{
    console.log(`${ip} matched: ${ip.match(ip_pattern) != null}`);
});

// 172.168.10.28 matched: true
// 192.18.1.233 matched: true
// 10.168.10.28 matched: true
// 8.8.0.8 matched: true
// 172:168:10:28 matched: false
// 172|168|10|28 matched: false

```
