# discourse-ht-nav
Load forum header/nav and footer from main Hearing Tracker site.

This only sets up discourse plugin structure and config -- content will be loaded on build (see below).

Discourse/plugin needs to be rebuilt upon main site header/footer changes.


## Populate header/footer connectors files
curl [MAIN SERVER HEADER/NAV ROUTE] > /var/www/discourse/plugins/discourse-ht-nav/assets/javascripts/discourse/templates/connectors/above-site-header/ht-header.hbs

curl [MAIN SERVER FOOTER ROUTE] > /var/www/discourse/plugins/discourse-ht-nav/assets/javascripts/discourse/templates/connectors/above-footer/ht-footer.hbs

* HT server credentials may be necessary (e.g. if connecting to staging)