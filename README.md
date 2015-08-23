### INSTALATION

node.js
```sh
npm install puntopagos-node
```

### HOW TO USE
```javascript
var puntoPagos = request('puntopagos-node');

// Config
puntoPagos.config('PUNTOPAGOS_KEY_CONFIG', 'PUNTOPAGOS_SECRET_CONFIG') 

// Create payment
puntoPagos.pay(puntoPagos.generateId(), amont, puntoPagos.paymentMethod.webpay, callback(err, data));
// data = {token:token, redirect:redirect}

// Validate payament
puntoPagos.validate(token, generated_id, amount, callback(err, data)); 
```

### PuntoPagos Documentation
[Oficial documentation](https://github.com/PuntoPagos/documentacion)
