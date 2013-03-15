phpBB installer
================

This is a simple Composer package that will install phpBB at the root of your Composer project.

phpBB is not directly contained in this project. It is downloaded from the phpbb.com website.


Installing phpBB using this Composer package:
----------------------------------------------

Not used to Composer? The first step is installing Composer. 
This is essentially a one line process:

```bash
curl -s https://getcomposer.org/installer | php
```

Windows users can download the phar file here: [http://getcomposer.org/download/](install composer).
Then create a *composer.json* file at the root of your project:

```json
{
    "require": {
        "sergeym/phpbb": "~3.0"
    }
}
```

and finally, run

```bash
php composer.phar install
```

This will download and unpack the phpBB archive at the root of your project.
In this example, the version downloaded is 3.0 or greater, but lower than 4.0 (this is the meaning of the ~ just before the version number).
