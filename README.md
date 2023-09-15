# AsteroidOS Hello World App
A simple hello world app for [AsteroidOS](http://asteroidos.org/)

See https://wiki.asteroidos.org/index.php/Creating_an_Asteroid_app for instruction on how to build and run it.

If you have used the Hello World App as a template and wish to use it as the basis for your own AsteroidOS application here are the steps:

 1. Decide on a name for your project, (we use `myproject-name` as an example here)
 2. Change the project name in `CMakeLists.txt` from `asteroid-helloworld` to your name (e.g. `myproject-name`)
 3. Rename the `i18n/asteroid-helloworld.desktop.h` file to user your project name (e.g. `i18n/myproject-name.desktop.h`)
 4. Rename the `asteroid-helloworld.desktop.template` file to use your project name (e.g. `myproject-name.desktop.template`)
 5. Edit the newly renamed `destkop.template` file from the previous step and change the `Exec=` line to your project name
 6. Optionally, but highly recommended, change the `Icon`, `X-Asteroid-Center-Color` and `X-Asteroid-Outer-Color` values in that same file
 7. Alter the functionality to suit


Note that for steps 3 and 4, use `git mv` to rename the files so that your repository will reflect these changes.
