# Ourchive Themes

This repo holds themes used in [ourchive](https://github.com/c-e-p/). 

We follow UIKit's [documentation](https://getuikit.com/docs/sass) for creating & modifying a theme using Sass. The assumption is that you will have a subdirectory, within this repo, containing the UIKit source from Git.

Compiled CSS is then added to the project by the developer.

Icons are currently in the ourchive repo and can be added to your uikit repo locally, following UIKit's [documentation](https://getuikit.com/docs/custom-icons). 

Ubuntu CLI to compile without copying custom icons (assumes you have Sass installed):

```sass ourchive-dark.scss > ourchive-dark.css && cp ourchive-dark.css /home/imp/projects/ourchive/ourchive_app/frontend/static/frontend/css/ourchive-dark.css && sass ourchive-light.scss > ourchive-light.css && cp ourchive-light.css /home/imp/projects/ourchive/ourchive_app/frontend/static/frontend/css/ourchive-light.css```

To compile and copy custom icons (assumes you have Sass & pnpm installed):

```cd uikit/ && pnpm compile && cd ../ && sass ourchive-dark.scss > ourchive-dark.css && cp ourchive-dark.css /home/imp/projects/ourchive/ourchive_app/frontend/static/frontend/css/ourchive-dark.css && sass ourchive-light.scss > ourchive-light.css && cp ourchive-light.css /home/imp/projects/ourchive/ourchive_app/frontend/static/frontend/css/ourchive-light.css```

This also assumes your directory structure has the uikit repo clone directly inside of the parent repo folder (ourchive-themes).
