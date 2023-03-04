# How to create your own Strapi template

## Introduction

In this article, you will go through the steps on how to create your own Strapi template and share it with the community.

### What is Strapi?

[Strapi is the leading open-source headless Content Management System (CMS)](https://strapi.io). It is 100% Javascript, based on Node.js, and used to build RESTful APIs and GraphQL. It also has a cloud SAAS, ☁ [Strapi Cloud](https://strapi.io/cloud) ☁ - a fully managed, composable, and collaborative platform to boost your content velocity!

Strapi enables developers to build projects faster with a flexible and customizable platform for managing content. Check out the Strapi Quickstart guide for a brief intro.

One of the benefits of Strapi is that developers can create and share their own templates for others to use.

### What is a Strapi Template?

A [Strapi template](https://docs.strapi.io/dev-docs/templates) is a pre-made Strapi configuration that allows to you to bootstrap a custom Strapi application in one go. A template can configure [collection types and single types](https://docs.strapi.io/user-docs/content-type-builder), [components and dynamic zones](https://docs.strapi.io/dev-docs/backend-customization/models), and [plugins](https://docs.strapi.io/dev-docs/plugins/plugins-intro).

Templates can be useful in saving you time and getting up and running with a project. You can make templates for all sorts use cases. These include:
- Blog sites
- Ecommerce sites
- Corporate sites
- Personal sites

In this tutorial, you will make a Strapi template for a blog site. These instructions don't just apply to blogs, but can be used for ecommerce, corporate, personal and other sites as well.

If you are in a rush and want to test out the template here's the source code for the template:

- [**Source Code**](https://github.com/Marktawa/strapi-template-blog)

## Prerequisites

Before we begin, make sure you have the following software installed on your machine:

- [Node v14.xx to v18.xx (LTS version)](https://nodejs.org/en/download/)
- [Git](https://git-scm.com/downloads)

## Step 1: Create a standard Strapi app

The first step is to create a standard Strapi application. You can do this by running the following command in your terminal:

```
npx create-strapi-app my-app --quickstart

```

> **NOTE**: *Replace `my-app` with the name of your application.*

This creates your Strapi app in the folder named `my-app`. The `--quickstart` flag sets up your Strapi app with an [SQLite](https://www.sqlite.org/index.html) database and automatically starts your server on port `1337`. 

Visit `http://localhost:1337/admin` in your browser and register your details in the Strapi Admin Registration Form.



## Step 2: Customize the Strapi app

The next step is to customize the Strapi application by creating e-commerce template collections. This will involve creating content types, fields, and relationships that will serve as the foundation of your Strapi template.

## Step 3: Test the Strapi app

Before generating your Strapi template, you will need to test your application to ensure that it works as intended. Test your application by running the following command in your terminal:

```
npm run develop

```

This will start a development server that you can use to preview your Strapi application.

## Step 4: Generate the Strapi template

Once you have tested and customized your Strapi application, you can generate a template by running the following command in your terminal:

```
npm run strapi generate:template --apiTemplate=api --adminTemplate=admin --pluginName=my-template

```

Replace `my-template` with the name of your template.

## Step 5: Configure the template

After generating your Strapi template, you will need to configure it by modifying the template's `package.json` file. This file contains metadata about your template, such as its name, version, and dependencies.

## Step 6: Publish the template

Once you have configured your Strapi template, you can publish it to the npm registry or to a private npm registry. You can do this using the following command:

```
npm publish --access public

```

## Step 7: Test the template

After publishing your Strapi template, you should test it to ensure that it works as intended. You can do this by creating a new Strapi application using your template and testing its functionality.

## Step 8: Deployment

Finally, you can deploy your Strapi template to a hosting provider, such as Heroku or AWS, to make it accessible to the wider community.

## Recommendations

When creating a Strapi template, it's important to follow best practices and maintain good documentation. This will make it easier for others to use your template and contribute to its development.

## Conclusion

Creating your own Strapi template can be a rewarding experience that allows you to share your knowledge and expertise with the wider community. By following the steps outlined in this article, you can create a high-quality Strapi template that others can use to build their own applications.