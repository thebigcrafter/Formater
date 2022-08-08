## Pre-requisites
- A bash shell (Windows Powershell is sufficient for Windows)
- [PHP 8.0](https://www.php.net/downloads.php) or newer available in your shell
- [NodeJS 16.16.0 LTS](https://nodejs.org/en/download) or newer available in your shell
- [Composer](https://getcomposer.org/download) available in your shell

## Windows Powershell (Run As Administrator)
Just do this step for the first time
```
$ Set-ExecutionPolicy -Scope CurrentUser -ExecutionPolicy RemoteSigned

Execution Policy Change
The execution policy helps protect you from scripts that you do not trust. Changing the execution policy might expose
you to the security risks described in the about_Execution_Policies help topic at
https:/go.microsoft.com/fwlink/?LinkID=135170. Do you want to change the execution policy?
[Y] Yes  [A] Yes to All  [N] No  [L] No to All  [S] Suspend  [?] Help (default is "N"): _

$ A

$ npm i -g npm yarn
```

## PHP-CS-Fixer
```shell
$ composer install
$ php vendor/bin/php-cs-fixer fix src
```

## Prettier
```shell
$ yarn
$ yarn run format
$ yarn run check
```
