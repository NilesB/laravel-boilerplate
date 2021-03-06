# Laravel Boilerplate

This is our internal boilerplate for Laravel projects, it should hopefully reduce the time it takes for you to setup a project & also improve code standards across the board.

## Installation

The Langley Foxall Laravel Boilerplate can be easily installed using Composer. Just run the following command and it will create a new directory for your project.

```bash
composer create-project langleyfoxall/laravel-boilerplate
```

The boilerplate and all its dependencies will be automatically downloaded.

## Features

The table below illustrates the planned features and the currently implemented features.

| Feature                                                           | Implemented | Desc                                |
| ------------------------------------------------------------------|:-----------:|:------------------------------------|
| [Log Viewer](https://github.com/rap2hpoutre/laravel-log-viewer)   | ✅          | Easily viewing logs                 |
| [React](https://github.com/facebook/react)                        | ✅          | Frontend framework                  |
| [ESLint](https://github.com/airbnb/javascript)                    | ✅          | Coding standards                    |
| [Ziggy](https://github.com/tightenco/ziggy)                       | ✅          | Use named routes in your js         |
| [JWT Auth](https://github.com/tymondesigns/jwt-auth)              | ✅          | JWT API authorization               |
| [Jest](https://github.com/facebook/jest)                          | ✅          | JS testing framework                |
| [Enzyme](https://github.com/airbnb/enzyme)                        | ✅          | Utilities for testing React         |
| [Travis](https://travis-ci.com/)                                  | ✅          | Continuous integration              |
| [Dusk](https://laravel.com/docs/5.6/dusk)                         | ✅          | Browser testing for Laravel (blade) |
| [Laravel Debug Bar](https://github.com/barryvdh/laravel-debugbar) | ✅          | Help debugger                       |

### Notes

- Be careful when using Jest & Dusk, they should not be used in tandem, use Jest & Enzyme for React rendered apps & Dusk for Blade rendered apps.
- When using Ziggy, ensure you add ```@routes``` before you include your application's bundle.
- JWTAuth is using the latest release candidate & not ```0.5.*```. Therefore make sure you use this link when referring to the docs. http://jwt-auth.readthedocs.io/en/develop/
- Travis (`.travis.yml`) may need some modifications based on your setup.
