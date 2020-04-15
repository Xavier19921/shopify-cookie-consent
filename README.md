# Shopify cookie consent
Cookie consent implementation for Shopify stores

The cookie consent implementation is built around <a href="https://cookieconsent.insites.com/" target="_blank">Insites' cookie consent</a>.

### Installation
1. Add a new section to your theme called `cookie-consent`.
2. Replace content within the new section, with everything from <a href="https://github.com/Youfront/shopify-cookie-consent/blob/master/cookie-consent.liquid">`cookie-consent.liquid`</a>.
3. Insert `{% section 'cookie-consent' %}` in your theme.liquid. Ideal placement is right before the closing of your body tag.
4. Use the theme customizer in your to style and enable the section.
