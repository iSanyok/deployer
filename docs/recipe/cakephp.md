<!-- DO NOT EDIT THIS FILE! -->
<!-- Instead edit recipe/cakephp.php -->
<!-- Then run bin/docgen -->

# cakephp

[Source](/recipe/cakephp.php)



* Requires
  * [common](/docs/recipe/common.md)

## Configuration
### shared_dirs
[Source](https://github.com/deployphp/deployer/blob/master/recipe/cakephp.php#L13)

Overrides [shared_dirs](/docs/recipe/common.md#shared_dirs) from `recipe/common.php`.

CakePHP 4 Project Template shared dirs

```php title="Default value"
[
    'logs',
    'tmp',
]
```


### shared_files
[Source](https://github.com/deployphp/deployer/blob/master/recipe/cakephp.php#L19)

Overrides [shared_files](/docs/recipe/common.md#shared_files) from `recipe/common.php`.

CakePHP 4 Project Template shared files

```php title="Default value"
[
    'config/.env',
    'config/app.php',
]
```



## Tasks

### deploy:init
[Source](https://github.com/deployphp/deployer/blob/master/recipe/cakephp.php#L27)



Create plugins' symlinks


### deploy:run_migrations
[Source](https://github.com/deployphp/deployer/blob/master/recipe/cakephp.php#L34)



Run migrations


### deploy
[Source](https://github.com/deployphp/deployer/blob/master/recipe/cakephp.php#L43)



Main task


This task is group task which contains next tasks:
* [deploy:prepare](/docs/recipe/common.md#deployprepare)
* [deploy:vendors](/docs/recipe/deploy/vendors.md#deployvendors)
* [deploy:init](/docs/recipe/cakephp.md#deployinit)
* [deploy:run_migrations](/docs/recipe/cakephp.md#deployrun_migrations)
* [deploy:publish](/docs/recipe/common.md#deploypublish)


