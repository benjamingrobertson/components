# Component Based Development Using UI_Patterns
A training workshop for people who develop websites using the component based approach.

## Local Environment Setup (Do this first)
Before anything else, follow these steps to get your local envrionment setup.

## Option 1 (Basic)
If you already have a system for creating a new Drupal 8 site locally (i.e. MAMP, LAMP, WAMP, AcquiaDev Desktop, etc.), you can go ahead and use that then follow these instructions:

1. Download and install the latest version of Drupal 8
2. Download and enable the following modules and their dependencies:
    * [Components Libraries](https://www.drupal.org/project/components)
    * [UI_Patterns](https://www.drupal.org/project/ui_patterns) (enable all submodules except field groups)
    * [Display Suite](https://www.drupal.org/project/ds)
    * [Paragraphs](https://www.drupal.org/project/paragraphs)
    * [Entity Reference Revisions](https://www.drupal.org/project/entity_reference_revisions)
    * [Devel](https://www.drupal.org/project/devel)
    * [Admin Toolbar](https://www.drupal.org/project/admin_toolbar)

3. Clone or download this repo anywhere on your machine
```
git clone https://github.com/mariohernandez/components
```

4. Copy the **nashville** theme from the repo into your drupal's `/themes/custom/`

5. Make the **nashville** theme your default theme

6. Clear your caches.



## Option 2 (Advanced)

1. Install Lando

For Mac OS, download the latest version on [GitHub](https://github.com/lando/lando/releases).  You can also [install Lando on other platforms](https://docs.devwithlando.io/installation/installing.html)


2. Install Composer

  * [Follow these instructions](https://getcomposer.org/doc/00-intro.md#installation-linux-unix-osx) for your specific Operating System
  * Great YouTube [tutorial on installing and using composer](https://www.youtube.com/watch?v=BnIZVHmROkk).


3. Clone or download this repo anywhere on your local machine

```
git clone https://github.com/mariohernandez/components
```


4. Start Lando

Change into the directory of the repo to run all commands below:

```
lando start
```

5. Install all PHP Dependencies with Composer

```
lando composer install
```


6. Install Drupal

`lando drush site-install config_installer --account-name=admin --account-pass=admin --db-url='mysql://drupal8:drupal8@database/drupal8' --site-name=Components`

7. Train your dragon.

## Enable the use of field templates within Display Suite
* Click Structure | Display Suite | Settings
* Under Field Templates check the box for **Enable Field Templates**
* Click **Save configuration**


## Training Material (work in progress)

For your convenience we have compiled [all training material](https://mariohernandez.gitbooks.io/components/content/), including step by step exercises in a gitbook.
This will be the official material we will use during training and it's currently being tested and refined.
