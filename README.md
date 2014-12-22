# Kwik Deploy #

Deploy your git based plugin to the subversion based WordPress plugin respository.

## Installation ##

`cd` to your plugin's root directory

~~~
git clone https://github.com/kevinchappell/kwik-deploy.git
~~~

## Usage ##

From the root of your plugin directory execute the deploy script passing your plugin's slug as the argument. For example if your plugin's URL is `https://wordpress.org/plugins/plugin-slug/` you would type the following:

~~~
./kwik-deploy/deploy.sh "plugin-slug"
~~~
