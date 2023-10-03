# Ourchive Themes

This repo holds themes used in [ourchive](https://github.com/c-e-p/). 

We follow UIKit's [documentation](https://getuikit.com/docs/sass) for creating & modifying a theme using Sass. The assumption is that you will have a subdirectory, within this repo, containing the UIKit source from Git.

Compiled CSS is then added to the project by the developer.

Icons are in the `custom/` folder and should be moved to the correct location (`uikit/custom`) after you clone UIKit, following the [documentation](https://getuikit.com/docs/custom-icons). 

Ubuntu CLI to compile without copying custom icons (assumes you have Sass installed):

```sass ourchive-dark.scss --style=compressed > ourchive-dark.css && cp ourchive-dark.css /path/to/repo/ourchive/ourchive_app/frontend/static/frontend/css/ourchive-dark.css && sass ourchive-light.scss --style=compressed > ourchive-light.css && cp ourchive-light.css /path/to/repo/ourchive/ourchive_app/frontend/static/frontend/css/ourchive-light.css```

To compile and copy custom icons (assumes you have Sass & pnpm installed):

```cd uikit/ && pnpm compile && cd ../ && sass ourchive-dark.scss --style=compressed > ourchive-dark.css && cp ourchive-dark.css /path/to/repo/ourchive/ourchive_app/frontend/static/frontend/css/ourchive-dark.css && sass ourchive-light.scss --style=compressed > ourchive-light.css && cp ourchive-light.css /path/to/repo/ourchive/ourchive_app/frontend/static/frontend/css/ourchive-light.css```

This also assumes your directory structure has the uikit repo clone directly inside of the parent repo folder (ourchive-themes).

# Credit

Custom icons are pulled from [The Noun Project](https://thenounproject.com):

* Night mode switcher by [Anggara Putra](https://thenounproject.com/angputra/)
* All other icons by[Shmidt Sergey](https://thenounproject.com/browse/collection-icon/cutiecons-32px-grid-2px-stroke-19102/?p=1)