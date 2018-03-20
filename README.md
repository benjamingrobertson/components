# Component Based Development Using UI_Patterns
A training workshop for people who develop websites using the component based approach.

## Local Environment Setup (Do this first)
Before anything else, follow these steps to get your local envrionment setup.

1. Clone or download this repo anywhere on your local machine

`git clone https://github.com/mariohernandez/components`

2. Initialize Lando. Accept defaults.

`lando init --recipe drupal8`

3. Start Lando

`lando start`

3. Install Drupal

`lando drush site-install config_installer --account-name=admin --account-pass=admin --db-url='mysql://drupal8:drupal8@database/drupal8' --site-name=Components`

5. Train your dragon.

## Training Documentation

[Training material](https://mariohernandez.gitbooks.io/components/content/), including step-by-step exercises, are available as a gitbook.  Proceed to the documentation after following the Environment setup instructions above.
