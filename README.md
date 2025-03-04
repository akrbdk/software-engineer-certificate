# software-engineer-certificate
Software Engineer Certificate

### 1 Growth in 2 Dimensions (php)

```php
function countMax($upRight) {
    $rows = [];
    $cols = [];
    
    foreach($upRight as $coord){
        list($r, $c) = explode(' ', $coord);
        $rows[] = $r;
        $cols[] = $c;
    }
    
    return min($rows) * min($cols);
}
$fptr = fopen(getenv("OUTPUT_PATH"), "w");
```

### 2 Relative pay (sql)

```sql
SELECT t1.NAME AS name1, t2.NAME AS name2
FROM Employee as t1
INNER JOIN Employee AS t2 ON t1.SALARY < t2.SALARY AND t1.NAME != t2.NAME
ORDER BY t1.ID ASC, t2.SALARY ASC;
```

### 3 REST API: IP Tracker (node.js)

```node
const fetch = require('node-fetch');

async function getCountryByIP(ip) {
    const url = https://jsonmock.hackerrank.com/api/ip?ip=${ip};

    try {
        const response = await fetch(url);
        const ans = await response.json();
        if (ans.total > 0) {
            return ans.data[0].country;
        } else {
            return 'No country information available for this IP';
        }
    } catch (error) {
        console.error('Error fetching IP data:', error);
        return 'Error occurred while fetching country information';
    }
}

const example_ip = '172.217.20.46';
getCountryByIP(example_ip).then(country => {
    console.log('Country of origin:', country);
});
```

### Certificate

![Certificate](https://github.com/akrbdk/software-engineer-certificate/blob/2c5ec4e39d50003ccfdead86632ea3c51d5f008d/software_engineer%20certificate.png)
