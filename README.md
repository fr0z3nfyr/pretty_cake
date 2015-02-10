# CakePHP: Cake Bake Console Theme for apps using Bootstrap [Alpha]
A personal theme for baking custom views, when app uses Twitter Bootstrap to perform user interface.

## Requirements 
This template theme is for Cake Bake Utility of [CakePHP 2.x](http://cakephp.org/) (for now, only testing on 2.5.6).

* Resources
  * [Bootstrap 3.x](http://getbootstrap.com/) (for now, only testing on 3.3.2)
  * [Font Awesome 4.x](http://fontawesome.io/) (for now, only testing on 4.2.0)

You should include Cascading Style Sheets (\*.css), JavaScript (\*.js) and Font resources in your layout(s).

## Installation
### GIT submodule
> Use this option if you wanna get the last work.

In your **app** directory, type:

    git submodule add https://github.com/nelson6e65/bake_bootstrap.git Console/Templates/bake_bootstrap
    git submodule init
    git submodule update

#####Note:
You can use another name instead of `bake_bootstrap` :wink:. For example, if you wanna use just `bootstrap`, the run insted:

    git submodule add https://github.com/nelson6e65/bake_bootstrap.git Console/Templates/bootstrap
    git submodule init
    git submodule update

### Manual
* Download lastest [zip](https://github.com/nelson6e65/bake_bootstrap/archive/master.zip) or [release](https://github.com/nelson6e65/bake_bootstrap/releases).
* Decompress it. You will get a  folder.
* Rename the resulting folder to `bake_bootstrap`.
* Move it under your templates directory (`app/Console/Templates/{here}`).

#####Note:
You can use another name instead of `bake_bootstrap`. For example, if you wanna use just `bootstrap`, then rename folder to `bootstrap`. :wink:

## Usage
Once you installed, you are able to make bootstraped views with [bake](http://book.cakephp.org/2.0/en/console-and-shells/code-generation-with-bake.html). :smiley:

You just need to pass `-t` (`--theme`) argument to `cake bake`:

    $ cake bake [subcommand] [-h] [-v] [-q] [-c default] [-t]

On Windows, you can run:

    $ cd path/to/cakephp/app
    $ .\Console\cake bake -t "bake_bootstrap"

If you don't pass `--theme` argument (or you typed a wrong template name), bake will ask you (at end) which template to use:

    ---------------------------------------------------------------
    You have more than one set of templates installed.
    Please choose the template set you wish to use:
    ---------------------------------------------------------------
    1. bake_bootstrap
    2. default
    Which bake theme would you like to use? (1/2)
    [1] >

Then, choose `bake_bootstrap` (`1` in this example) and press Enter to continue. :satisfied:

#####Note:
*If you changed the default theme name* (`bake_bootstrap`), you must run `$ .\Console\cake bake -t "{theme_name}"`  command instead (or select `{theme_name}` when bake ask you), where `{theme_name}` means your personalized name :wink:.

Example: For `bootstrap` theme name, you should run instead:

    $ .\Console\cake bake -t "bootstrap"

## Instructions FAQ

**What means `path/to/cakephp/app`?**
> [See below].

**What means `app directory`?**
> Is de root path of your application. That is, by default, the **app** subdirectory of your CakePHP installation directory.
> 
For example, using wamp on Windows, *app directory* should be `C:\wamp\www\cakephp\app\` (if you installed CakePHP in `C:\wamp\www\cakephp\`).
> For further info, check [CakePHP Folder Structure](http://book.cakephp.org/2.0/en/getting-started/cakephp-folder-structure.html#the-app-folder).

**Where are located console themes?**
> Console themes are placed inside your `app / Console / Templates /` directory:
> 
`path/to/cakephp/app/Console/Templates/{here}`
> For further info, check [CakePHP Folder Structure](http://book.cakephp.org/2.0/en/getting-started/cakephp-folder-structure.html#the-app-folder).

**Where should be located this theme?**
> As I said in install instructions, content of this theme *must* be located inside templates directory: `app / Console / Templates / {theme_name} /`.
The default `{theme_name}` is `bake_bootstrap`:
>
`path/to/cakephp/app/Console/Templates/bake_bootstrap/`

**What is Git submodule?**
> Is a Git tool to treat the two projects as separate yet still be able to use one from within the other. Check this page: http://git-scm.com/book/en/v2/Git-Tools-Submodules

## TODO List
### View actions
- [ ] Personalize 'index' view
- [x] Personalize 'view' view 
- [ ] Personalize 'add' view
- [ ] Personalize 'edit' view
- [ ] Add 'delete' view (?)
- [ ] Add 'find' view

### Controller actions
- [ ] Personalize 'delete' action
- [ ] Add 'delete' action

##Licence
Licensed under The MIT License (MIT). Check [LICENSE](/LICENSE) for full copyright and license information.
