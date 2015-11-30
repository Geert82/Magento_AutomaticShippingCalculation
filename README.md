# Magento_AutomaticShippingCalculation

This extension automatically applies shipping based on 3 parameters:

COUNTRY:
When a customer first go to the shopping cart, shipping method is calculated using the store’s default country (System->Configuration->General->Countries Options->Default Country).

If the customer is logged in, the country of the customer’s shipping address is used.
If a customer selected a country and clicked ‘get quote’, the selected is used.

SORT ORDER:
Sort order of shipping methods can be set up at System->Configuration->Shipping Methods->Shipping Method Name->Sort Order Shipping method has the smallest sort order value will get applied.

For examle,
Set Free shipping to have a sort order of 1, Flat Rate to have a sort order of 2.
When freeshipping is available, it will be applied. When it is not available, flat rate is applied.

POSTALCODE
When a customer first go to the shopping cart, shipping method is calculated using the store’s default postalcode (System->Configuration->Sales->Shipping Settings->ZIP/Postal Code).

If the customer is logged in, the postalcode of the customer’s shipping address is used.
If a customer selected a postalcode and clicked ‘get quote’, the selected is used.


Shipping rates will get recalculated when the customer:
  - add items to cart
  - update items in cart
  - remove items from cart
