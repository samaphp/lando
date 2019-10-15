# Lando config file for Drupal 8

[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](http://makeapullrequest.com)
[![Support Lando](https://img.shields.io/badge/Support-Lando-f06292.svg)](https://www.patreon.com/devwithlando)

My custom Lando config file for Drupal 8. It is contain these services:
- Latest PHP version supported by Drupal 8. (PHP 7.3).
- MySQL 5.7.27
- Using Drush command from local path.
- Mailhog to receive all emails sent using the Mailhog SMTP port. (Require drupal/smtp contrib module and setup the proper SMTP port).
- Xdebug the debugger and profiler tool for PHP. Can be integrated with PHPStorm [Configuring PHPStorm](https://www.drupal.org/docs/develop/development-tools/configuring-phpstorm).

## Custom commands
- `lando abracadabra`: Used when you cloned the Drupal 8 project from your repository. This command will automate the installation and importing all configs from (sync) folder.
- `lando dejavu`: This command will help you to import and apply any new changes have been made since last `git pull` time.
- `lando locale`: This command will import all new locale changes from the .po files in your project.

Also, this config file has a demo of custom commands that will run post-start and pre-destroy.

I will keep maintining this repo and will add updates that makes my development automated and easier.


Big thanks to Lando creators 🏆 Please consider supporting them on [Patreon](https://www.patreon.com/devwithlando).
