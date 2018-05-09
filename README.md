# Shopify cookie consent
Cookie consent implementation for Shopify stores

The cookie consent implementation is built around <a href="https://cookieconsent.insites.com/" target="_blank">Insites' cookie consent</a>.

## Installation
1. Add cookie-consent.liquid to your theme's sections.
2. Include cookie-consent.liquid in your theme.liquid. Ideal placement is right before the closing of your body tag.
3. Translate language strings in your theme language.
4. Use the theme customizer in your Shopify store backend to style and enable the section.

## Compliance
<b>NOTICE</b>: Compliance currently only works for the <a href="https://help.shopify.com/manual/reports-and-analytics/google-analytics" target="_blank">Google Analytics integration 

To use compliance feature, you will need to add additional JavaScript to your Analytics snippet. Add the following snippet to "Custom JavaScript"

```
var UA = 'UA-XXXX-Y';
if (document.cookie.indexOf('ga-disable-' + UA + '=true') > -1) {
  window['ga-disable-' + UA] = true;
}
```

Replace `UA-XXXX-Y` with your Analytics tracking code.