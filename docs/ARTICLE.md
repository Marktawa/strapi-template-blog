# How to create your own Strapi template

## Introduction

In this article, you will go through the steps on how to create your own Strapi template and share it with the community.

### What is Strapi?

[Strapi is the leading open-source headless Content Management System (CMS)](https://strapi.io). It is 100% Javascript, based on Node.js, and used to build RESTful APIs and GraphQL.

Strapi enables developers to build projects faster with a flexible and customizable platform for managing content. Check out the Strapi Quickstart guide for brief intro.

One of the benefits of Strapi is that developers can create and share their own templates for others to use. 

## Prerequisites

Before we begin, make sure you have the following software installed on your machine:

- [Node v14.xx to v18.xx (LTS version)]()
- Git

## Step 1: Create a standard Strapi app

The first step is to create a standard Strapi application. You can do this by running the following command in your terminal:

```
npx create-strapi-app my-app --quickstart

```

Replace `my-app` with the name of your application.

## Step 2: Customize the Strapi app (e-commerce template collections)

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