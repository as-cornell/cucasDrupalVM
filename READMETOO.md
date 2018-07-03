
#Installation Instructions

##Install Virtualbox && Vagrant for MacOSX
https://gist.github.com/tomysmile/0618f1aa16341706940ed36b423b431c
```
vagrant plugin install vagrant-hostsupdater
```
Clone this repo into ~sites/drupal-vm-cd
Run ```composer install``` from ~sites/drupal-vm-cd
Clone https://github.com/as-cornell/cucas8zlatan into ~sites/drupal-vm-cd/docroot
Run ```composer install``` from ~sites/drupal-vm-cd/docroot
Run ```vagrant up --provision`` from ~sites/drupal-vm-cd

##Drupal VM Quick start guide
https://github.com/geerlingguy/drupal-vm#quick-start-guide

##Drupal VM as a Composer Dependency
http://docs.drupalvm.com/en/latest/deployment/composer-dependency/
