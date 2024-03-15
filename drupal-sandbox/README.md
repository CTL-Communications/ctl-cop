# Drupal Installation

1. Install Lando on your computer, follow our [Lando Installation Guide](https://ctlcomms.atlassian.net/wiki/spaces/COP/pages/106201092/Site+building+-+Drupal+Introduction+Installation+and+major+subsystems#Install-Lando)
2. Clone this project onto your local machine
```shell
git clone git@github.com:CTL-Communications/ctl-cop.git
```
3. Open your terminal and navigate to the drupal-sandbox directory.
```shell
 cd ctl-cop/drupal-sandbox
```
4. Start the site
```shell
lando start
```
5. Install the site
```shell
lando install
```
6. Open the site in your browser. You will get a screen saying that the connection is not private. Just ignore it and click Continue :)
Be patient while it loads, might take around 15-30 seconds.
[https://drupal-sandbox.lndo.site/](https://drupal-sandbox.lndo.site/)

7. Login as an Administrator with the following credentials, happy learning!
```shell
  username: admin
  password: drupal
```
