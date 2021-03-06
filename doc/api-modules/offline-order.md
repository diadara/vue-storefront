# Wishlist module

The offline order module as name suggests is a set of mixins responsible for support for offline orders. You can find methods responsible for confirming/canceling orders placed offline.

## Content

#### confirmOrder
- [method] confirmOrder()

#### cancelOrder
- [method] cancelOrder()

## Helpers

#### onNetworkStatusChange
- [function] onNetworkStatusChange(store)

## Extends

- `service-worker.js` - for offline notifications

## Example

````javascript
// Inside Vue component
import {
  confirmOrder,
  cancelOrder
} from '@vue-storefront/core/api/offline-order'

export default {
  //...other properties
  mixins: [
    confirmOrder,
    cancelOrder
  ]
}
````
