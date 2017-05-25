# node-csgo-tm
API library for csgo.tm market

[Documentation](https://github.com/Yashko/node-csgotm/wiki)

Based on https://github.com/Yashko/node-csgotm/

***

New API method: 

```javascript
var csgotm = require('csgo-tm');
var market = new csgotm('apiKey');

var item = 'new_[classid]_[instanceid]';
var price = '[price]';

market.api.SetPrice(item, price, (err, data) => {
	if(err) return console.error(err);
	console.log(data);
});
```

More info about method: https://csgo.tm/docs/
