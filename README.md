# Drush from git master

You probably only want this cartridge if you want to run Drupal 8 on OpenShift.

Drush for Drupal 7 can be included by putting the following in depslist.txt of a PHP cartridge.

```
pear.drush.org/drush-6.0.0
```

### Pulling in new changes with `git subtree`

The initial import of Drush from master was done with this command:

```
git subtree add --prefix usr/drush git@github.com:drush-ops/drush.git master --squash
```

You can pull in new changes from Drush master with the following command:

```
git subtree pull --prefix usr/drush git@github.com:drush-ops/drush.git master --squash
```
