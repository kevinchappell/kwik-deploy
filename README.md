# Kwik Deploy

Deploy your plugin to the WordPress repo

## Who is this for?
This script if for anyone using Git for their plugin's source control that needs a fast way to push changes to the WordPress repository

## Installation

Kwik Deploy can be installed anywhere on your machine but to make it available to all your plugins you'll want to add it to your `$PATH`. First we'll start by cloning the project. In the below example we are cloning into the current user's (you) `bin`.

~~~
git clone https://github.com/kevinchappell/kwik-deploy.git ~/bin/kwik-deploy
~~~

To add to `$PATH` you can open your `~/.bashrc` and add `export PATH=$PATH:~/bin/kwik-deploy` line to the bottom of the file.

## Usage ##

From the root of your plugin directory run the deploy script passing your plugin's slug as the argument. For example if your plugin's URL is `https://wordpress.org/plugins/my-plugin-name/` you would type the following:

```
kwik-deploy my-plugin-name
```

### Note
If your plugin directory name is the same as your plugin's slug you don't need to pass the slug as an argument, the deploy script will use the directory name as the slug. Additionally if the directory name is My Plugin Name, MyPluginName, or My-Plugin-Name and any combination the deploy script should convert it to `my-plugin-name`. This should allow you to deploy your plugin to the WordPress repo simply by typing:
```
kwik-deploy
```
