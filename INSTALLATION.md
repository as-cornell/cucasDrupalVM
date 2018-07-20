# Installation Instructions

This project template provides a starter kit for managing your site
dependencies with [Composer](https://getcomposer.org/).

## Install Virtualbox and Vagrant for MacOSX

1. [Install Virtualbox and Vagrant](https://gist.github.com/tomysmile/0618f1aa16341706940ed36b423b431c)
1. Run `vagrant plugin install vagrant-hostsupdater`
1. Clone this repo into `~sites` and rename the folder `~sites/drupal-vm-cd`
1. Run `composer install` from `~sites/drupal-vm-cd`
1. Run `mkdir sites` and `cd sites`
1. If adding a new site, update `config.yml` to include a new `vagrant_synced_folders` block for your new directory under `~sites/drupal-vm-cd/sites/NEWSITENAME`
1. Clone [zlatan](https://github.com/as-cornell/cucas8zlatan) into `~sites/drupal-vm-cd/sites/NEWSITENAME`
1. Run `composer install` from `~sites/drupal-vm-cd/sites/NEWSITENAME`
1. Run `vagrant up --provision` from `~sites/drupal-vm-cd`
1. For multisite, create sites folder under `docroot/sites/SITENAME` and edit `docroot/sites/php`
1. Add another vhost block, mySQL database and user as described [here](http://docs.drupalvm.com/en/latest/deployment/multisite/)


## Drupal VM Quick start guide

[On github](https://github.com/geerlingguy/drupal-vm#quick-start-guide)

## Drupal VM as a Composer Dependency

[Drupal VM Documentation](http://docs.drupalvm.com/en/latest/deployment/composer-dependency/)

## Setting up Emulsify and Pattern Lab

[Four Kitchens / Emulsify at github](https://github.com/fourkitchens/emulsify)

### notes

1. Make sure Node and Ruby are updated via Homebrew [Homebrew help](https://docs.brew.sh/FAQ)
1. Make sure Node is running as ~ v 8.0.0 `node -v`  [Help](https://stackoverflow.com/questions/3987683/homebrew-install-specific-version-of-formula)
1. Run Emulsify script: `vagrant ssh` -> `cd docroot/themes/contrib/emulsify/` -> `php emulsify.php "THEME NAME"`
1. Outside of vagrant ssh: `cd docroot/themes/custom/THEME_NAME/` -> `yarn install`
1. Inside Vagrant ssh: `drush sa` to get @ALIAS -> `drush @ALIAS then THEME_NAME -y && drush @ALIAS en components unified_twig_ext -y`
1. Outside of vagrant ssh: `yarn start`
1. Inside Vagrant ssh: `drush @ALIAS cr`
1. Theme should now work, and Pattern Lab availible here: `http://localhost:3000/pattern-lab/public/`

:hankey: :fire: :cactus: :mountain_railway:
