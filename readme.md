# Installation Instructions
1) Install Virtualbox && Vagrant for MacOSX<br />
    https://gist.github.com/tomysmile/0618f1aa16341706940ed36b423b431c<br />
2) Clone this repo into ~sites/drupal-vm-cd<br />
3) Run 'composer install' from ~sites/drupal-vm-cd<br />
4) Clone https://github.com/as-cornell/cucas8zlatan into ~sites/drupal-vm-cd/docroot<br />
5) Run 'composer install' from ~sites/drupal-vm-cd/docroot<br />
6) Run 'vagrant up --provision' from ~sites/drupal-vm-cd<br />

#References
##Drupal VM Quick start guide
https://github.com/geerlingguy/drupal-vm#quick-start-guide

##Drupal VM as a Composer Dependency
http://docs.drupalvm.com/en/latest/deployment/composer-dependency/
