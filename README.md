# drupal8-graphql-scratchpad

Minimal setup to try GraphQL on Drupal8.

## How to Use

Install Drupal:

```
lando drush si --db-url=mysqli://drupal8:drupal8@database/drupal8 --account-pass admin -y
```

Install GraphQL Example module:

```
lando drush si pm:en graphql_example
```

Get the local site url:


```
lando info | grep http
```

Login at /user/login

Create a server at /admin/config/graphql, then open the explorer and try out
the example schema.
