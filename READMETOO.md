# Installation Instructions

This project template provides a starter kit for managing your site
dependencies with [Composer](https://getcomposer.org/).

## Install Virtualbox and Vagrant for MacOSX

1. [Install Virtualbox and Vagrant](https://gist.github.com/tomysmile/0618f1aa16341706940ed36b423b431c)
1. Run `vagrant plugin install vagrant-hostsupdater`
1. Clone this repo into `~sites/drupal-vm-cd`
1. Run `composer install` from `~sites/drupal-vm-cd`
1. Clone [cucas8zlatan](https://github.com/as-cornell/cucas8zlatan) into `~sites/drupal-vm-cd/sites/NEWSITENAME`
1. Run `composer install` from `~sites/drupal-vm-cd/docroot`
1. Run `vagrant up --provision` from `~sites/drupal-vm-cd`


## Drupal VM Quick start guide

[On github](https://github.com/geerlingguy/drupal-vm#quick-start-guide)

## Drupal VM as a Composer Dependency

[Drupal VM Documentation](http://docs.drupalvm.com/en/latest/deployment/composer-dependency/)
