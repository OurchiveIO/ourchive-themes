# Ourchive Themes

This repo holds themes used in [ourchive](https://github.com/c-e-p/). 

We use [Bootstrap](https://getbootstrap.com/docs/5.3/).

Recommended workflow: 

Clone the theme repo into a `theme` folder within your cloned Ourchive directory. Assumed folder structure:

````
- ourchive
-- ourchive_app
-- theme
-- .dockerignore
-- [other top-level files & directories]
````
Work out of the custom SASS in `scss/ourchive.scss`.

Compiled CSS is then added to the Django project by the developer:

`sass --watch ./scss/ourchive.scss ../ourchive_app/frontend/static/frontend/css/ourchive.css`

From there, assets are compiled and deployed like you would for any other Django project.

---

# Credit

** Note: this section is under construction. The below reflects icons used prior to Ourchive's 0.7.0 release. **

Custom icons are pulled from [The Noun Project](https://thenounproject.com):

* Night mode switcher by [Anggara Putra](https://thenounproject.com/angputra/)
* All other icons by[Shmidt Sergey](https://thenounproject.com/browse/collection-icon/cutiecons-32px-grid-2px-stroke-19102/?p=1)