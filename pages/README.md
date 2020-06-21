# PAGES

This directory contains your Application Views and Routes.
The framework reads all the `*.vue` files inside this directory and creates the router of your application.

More information about the usage of this directory in [the documentation](https://nuxtjs.org/guide/routing).

The file tree:

pages/
--| _slug/
-----| comments.vue
-----| index.vue
--| users/
-----| _id.vue
--| index.vue

Will handle requests like this:

模式	        匹配路径	    $route.params	    component
/:slug/comments	/gold/comments	{ slug: 'gold' }	pages/_slug/comments.vue
/users/:id	    /users/123	    { id: 123 }	        pages/users/_id.vue

This file tree:

pages/
--| people/
-----| _id.vue
-----| index.vue
--| _.vue
--| index.vue

Will handle requests like this:

Path	    File
/	        index.vue
/people	    people/index.vue
/people/123	people/_id.vue
/about	    _.vue
