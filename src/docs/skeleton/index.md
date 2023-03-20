# Skeleton

<!-- markdownlint-disable no-inline-html -->

Skeleton is a minimal but powerful MVC boilerplate built on top of Leaf. It's designed to be simple, fast and easy to use. It is meant to bring structure to your Leaf workflow without forcing you to stick to any framework. It is a good starting point for building lightweight applications using the MVC pattern.

::: tip Leaf MVC vs Leaf API vs Skeleton

Leaf offers three setups for you to choose from. You can find more information about these setups in the [MVC](/docs/mvc/#mvc-in-leaf) section.

:::

## Installation

The easiest way to setup Skeleton is to use the [Leaf CLI](/docs/cli/):

```bash
leaf create <project-name> --skeleton --v3
```

You can also setup a Skeleton app by using [Composer](https://getcomposer.org/):

```bash
composer create-project leafs/skeleton <project-name>
```

This command will set up a Skeleton app in the `<project-name>` directory. You can then run the app using the Leaf CLI:

```bash
cd <project-name>
leaf serve
```

Or the [built-in PHP server](https://www.php.net/manual/en/features.commandline.webserver.php):

```bash
cd <project-name>
php -S localhost:8000
```

You should then see the welcome page in your browser.

![Skeleton Welcome Page](https://user-images.githubusercontent.com/26604242/224507748-87396f4d-7b1e-4d61-ada1-b37e732c739b.png)

## Directory Structure

The Skeleton directory structure is setup to be straighforward and understandable at a glance. You can completely change the directory structure to suit your needs, just be sure to update the paths in the `config.php` file.

For a fresh Skeleton app, the directory structure looks like this:

```bash
C:.
├── config
├── controllers
├── models
├── pages
│   └── components
├── routes
├── storage
│   ├── app
│   │   └── public
│   ├── framework
│   │   └── views
│   └── logs
└── vendor
```

- ### The `config` directory

  The `config` directory contains the configuration files for your application. These are used to configure how Leaf and it's modules interact with your application. You can find more information about the configuration files in the [Configuration](/docs/mvc/config) section.

- ### The `controllers` directory

  The `controllers` directory contains the controllers for your application. These are used to handle HTTP requests. You can find more information about the controllers in the [Controllers](/docs/mvc/controllers) section.
  
- ### The `models` directory

  The `models` directory contains the models for your application. These are used to interact with the database. You can find more information about the models in the [Models](/docs/mvc/models) section.

- ### The `pages` directory

  The `pages` directory contains the views and frontend assets for your Leaf application.

- ### The `routes` directory

  The `routes` directory contains routes for your application. These are used to map HTTP requests to controllers. You can find more information about the routes in the [Routing](/docs/mvc/routing) section.

- ### The `storage` directory

  The `storage` directory contains the compiled views, logs and other files generated by your application. It's divided into a few sub-directories:

  - `app` - Contains the files generated by your application. This includes the compiled views and the files uploaded by users.
  - `framework` - Contains the framework generated files for your application.
  - `logs` - Contains the log files generated by your application.

- ### The `vendor` directory

  The `vendor` directory contains all the dependencies installed by Composer. It's automatically generated when you install the dependencies using Composer.

## Next Steps

Follow along with the next steps to learn more about Skeleton.

<div class="vt-box-container next-steps">
  <a class="vt-box" href="/docs/mvc/config">
    <h3 class="next-steps-link">Skeleton Configuration</h3>
    <small class="next-steps-caption">Learn how to configure Leaf and your app to work in different ways.</small>
  </a>
  <a class="vt-box" href="/docs/mvc/routing">
    <h3 class="next-steps-link">Routing</h3>
    <small class="next-steps-caption">Learn how routing works in your Leaf applications.</small>
  </a>
  <a class="vt-box" href="/docs/mvc/controllers">
    <h3 class="next-steps-link">Controllers</h3>
    <small class="next-steps-caption">Learn how to use controllers in your Leaf applications.</small>
  </a>
</div>