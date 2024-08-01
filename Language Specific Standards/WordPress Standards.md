We follow the set of standards set by WordPress for the development of WordPress core. They have a solid set of standards for all aspects of theme and plugin development, as well as documentation standards. Refer to the following resources for more information on the standards for each set of coding standards along with helpful resources.

- **HTML Standards**
	- [Official WordPress HTML Standards](https://developer.wordpress.org/coding-standards/wordpress-coding-standards/html/)
	- [W3C HTML Validator](https://validator.w3.org/)
- **CSS Standards**
	- [Official WordPress CSS Standards](https://developer.wordpress.org/coding-standards/wordpress-coding-standards/css/)
	- [Additional Guide on Idiomatic CSS](https://github.com/necolas/idiomatic-css)
- **JavaScript Standards**
	- [Official WordPress JS Standards](https://developer.wordpress.org/coding-standards/wordpress-coding-standards/javascript/)
	- [Documentation on Linting](https://contribute.jquery.org/style-guide/js/#linting)
- **PHP Standards**
	- [Official WordPress PHP Standards](https://developer.wordpress.org/coding-standards/wordpress-coding-standards/php/)
	- [PHP Documentation Standards](https://developer.wordpress.org/coding-standards/inline-documentation-standards/php/)
	- [PHP Linting Tools](https://github.com/WordPress/WordPress-Coding-Standards)

## Project Structure

Our WordPress themes and plugin follow set structures. Conveniently, most of these are automatically applied if you create the [theme](https://github.com/UCF/CM-WP-Theme-Template), [child-theme](https://github.com/UCF/CM-WP-Child-Theme-Template) or [plugin](https://github.com/UCF/CM-WP-Plugin-Template) using one of our GitHub templates. The general structures of the projects follows the requirements set out by WordPress for [themes](https://developer.wordpress.org/themes/core-concepts/theme-structure/) and [plugins](https://developer.wordpress.org/plugins/) with the addition of our particular process for building compiled assets, like SCSS and JavaScript files.

As a general rule, however, all of our themes and plugins should follow the same basic steps for development to reduce the amount of per-project knowledge needed in order to work on the project. Currently, our primary tool for automating the build process is [Gulp](https://gulpjs.com/), a NodeJS utility that allows for a series of tasks to be defined and run, either when triggered individually, grouped, or when changes occur to certain files. This tools allows a new developer on a project to follow a few simple steps and immediately have a working development environment for a theme or plugin. Here is an example of what those steps might be for a WordPress theme:

1. Clone the project into the `wp-contents/themes` directory of a local WordPress installation.
2. Install the NodeJS dependencies using `npm install`.
3. Copying the `gulp-config.template.json` to `gulp-config.json` and updating any values as desired.
4. Running `gulp watch`.

After just those 4 steps, a developer would be able to see any changes in their PHP, SCSS or JS files reflected on their local installation of the theme. The primary objective with this project setup is to keep projects **consistent**, **easy to get started with** and **easy to update**.

## Project Documentation


