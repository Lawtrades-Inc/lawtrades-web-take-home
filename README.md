# lt-take-home

## Project Directions
1. Your list is to take a list of job postings/ job opportunities and then display it nicely.
2. Here are the public APIs that are available for you to use:
```
https://lawtrades-be.herokuapp.com/v1/public/positions?status=Publish&page=0&limit=21&talentType[]=attorney&seniority[]=Senior&employmentType[]=Full-Time+%2F+Contract&minPayout=100&maxPayout=400

This is the simplest call, without pagination, that returns all positions published:
https://lawtrades-be.herokuapp.com/v1/public/positions?status=Publish

1. Notice that the above has the following options for when you are fetching the list of opportunities:
a. talentType filter, which can be one of the following: attorney, paralegal, legalOperations, compliance, administrator, and contractManager
b. seniority, which can be one of the following: junior, midLevel, senior
c. minPayout and maxPayout, minPayout >= 30, maxPayout <= 1000
d. employmentType, which can be one of the following: fullTime, partTime, contract, project
```
3. Each opportunity listed should be in a card-like format. It should have the title, description, and highlight the salary_rate, and whether or not it is part-time, etc..
4. Extra --- If you have time:
*  Make the site mobile responsive 
*  Add the ability to filter by seniority or talentTypes.
5. UI is important, but please focus more on completion and clean-coding over designs (this should be the last step of your work).

NOTE : PLEASE LIMIT YOURSELF TO NO MORE THAN 5 hours on this project. It should not take you that long and we don't want you to spend too much time on this project.
This was not the intention. We want to know about how you write/organize/and make decisions around code.
Packages and libraries that you think are appropriate are all fair game. We have Ant-Design as our chosen Library, but if you want to, feel free to pull in other UI libraries.

Walk us through the code and explain to us your choices. What types of tradeoffs did you make? If you had more time, what would you have done differently?

1. When you are finished, please share your github privately to the Lawtrades Team. We will then schedule some time to go over the project with you
2. Your project should be able to run by using 'yarn dev'. Please add documentation where appropriate.
3. The node version we are using is v16.17.0
4. Please use the instructions below to install and run the app

## Build Setup

```bash
# install dependencies
$ yarn install

# serve with hot reload at localhost:3000
$ yarn dev

# build for production and launch server
$ yarn build
$ yarn start

# generate static project
$ yarn generate
```

For detailed explanation on how things work, check out the [documentation](https://nuxtjs.org).

## Special Directories

You can create the following extra directories, some of which have special behaviors. Only `pages` is required; you can delete them if you don't want to use their functionality.

### `assets`

The assets directory contains your uncompiled assets such as Stylus or Sass files, images, or fonts.

More information about the usage of this directory in [the documentation](https://nuxtjs.org/docs/2.x/directory-structure/assets).

### `components`

The components directory contains your Vue.js components. Components make up the different parts of your page and can be reused and imported into your pages, layouts and even other components.

More information about the usage of this directory in [the documentation](https://nuxtjs.org/docs/2.x/directory-structure/components).

### `layouts`

Layouts are a great help when you want to change the look and feel of your Nuxt app, whether you want to include a sidebar or have distinct layouts for mobile and desktop.

More information about the usage of this directory in [the documentation](https://nuxtjs.org/docs/2.x/directory-structure/layouts).


### `pages`

This directory contains your application views and routes. Nuxt will read all the `*.vue` files inside this directory and setup Vue Router automatically.

More information about the usage of this directory in [the documentation](https://nuxtjs.org/docs/2.x/get-started/routing).

### `plugins`

The plugins directory contains JavaScript plugins that you want to run before instantiating the root Vue.js Application. This is the place to add Vue plugins and to inject functions or constants. Every time you need to use `Vue.use()`, you should create a file in `plugins/` and add its path to plugins in `nuxt.config.js`.

More information about the usage of this directory in [the documentation](https://nuxtjs.org/docs/2.x/directory-structure/plugins).

### `static`

This directory contains your static files. Each file inside this directory is mapped to `/`.

Example: `/static/robots.txt` is mapped as `/robots.txt`.

More information about the usage of this directory in [the documentation](https://nuxtjs.org/docs/2.x/directory-structure/static).

### `store`

This directory contains your Vuex store files. Creating a file in this directory automatically activates Vuex.

More information about the usage of this directory in [the documentation](https://nuxtjs.org/docs/2.x/directory-structure/store).
