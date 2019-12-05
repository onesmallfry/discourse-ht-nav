# discourse-ht-nav
Load forum header and footer from main hearing tracker site

## Populate header/footer connectors files
### Staging
curl -u USER:PASS https://staging.hearingtracker.com/forum_header > /var/www/discourse/plugins/discourse-ht-nav/assets/javascripts/discourse/templates/connectors/above-site-header/ht-header.hbs

curl -u USER:PASS https://staging.hearingtracker.com/forum_footer > /var/www/discourse/plugins/discourse-ht-nav/assets/javascripts/discourse/templates/connectors/above-footer/ht-footer.hbs

* replace USER & PASS with appropriate staging server credentials

### Production
curl https://www.hearingtracker.com/forum_header > /var/www/discourse/plugins/discourse-ht-nav/assets/javascripts/discourse/templates/connectors/above-site-header/ht-header.hbs

curl https://www.hearingtracker.com/forum_footer > /var/www/discourse/plugins/discourse-ht-nav/assets/javascripts/discourse/templates/connectors/above-footer/ht-footer.hbs
