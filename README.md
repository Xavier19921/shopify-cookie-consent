# Shopify cookie consent
Cookie consent implementation for Shopify stores

The cookie consent implementation is built around <a href="https://cookieconsent.insites.com/" target="_blank">Insites' cookie consent</a>.

### Installation
1. Add a new section to your theme called `cookie-consent`.
2. Replace content within the new section, with everything from <a href="https://github.com/Youfront/shopify-cookie-consent/blob/master/cookie-consent.liquid">`cookie-consent.liquid`</a>.
3. Insert `{% section 'cookie-consent' %}` in your theme.liquid. Ideal placement is right before the closing of your body tag.
4. Use the theme customizer in your to style and enable the section.

### Compliance
<b>NOTICE</b>: Compliance currently only works for the <a href="https://help.shopify.com/manual/reports-and-analytics/google-analytics" target="_blank">Google Analytics integration</a> 

To use compliance feature, you will need to add additional JavaScript to your Analytics snippet. Add the following snippet to "Custom JavaScript"

```js
var UA = 'UA-XXXX-Y';
if (document.cookie.indexOf('ga-disable-' + UA + '=true') > -1) {
  window['ga-disable-' + UA] = true;
}
```

Replace `UA-XXXX-Y` with your Analytics tracking code.
