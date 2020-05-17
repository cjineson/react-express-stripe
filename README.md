# react-express-stripe

Sample React/Express Stripe checkout
Based on https://www.robinwieruch.de/react-express-stripe-payment

=> backend/constants/stripe.js
```
const configureStripe = require('stripe');
 
const STRIPE_SECRET_KEY = process.env.NODE_ENV === 'production'
    ? 'sk_live_MY_SECRET_KEY'
    : 'sk_test_MY_SECRET_KEY';
 
const stripe = configureStripe(STRIPE_SECRET_KEY);
 
module.exports = stripe;
```

-> frontend/constants/stripe.js
```
const STRIPE_PUBLISHABLE = process.env.NODE_ENV === 'production'
  ? 'pk_live_MY_PUBLISHABLE_KEY'
  : 'pk_test_MY_PUBLISHABLE_KEY';
 
export default STRIPE_PUBLISHABLE;
```
