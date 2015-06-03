# sencha-hotfixes

Packages for each ExtJS / Sencha Touch version containing all hotfixes managed by Jarvus Innovations

## Supported frameworks
Hotfix packages are currently being maintained for:

- [touch-2.3.0](https://github.com/JarvusInnovations/sencha-hotfixes/tree/touch-2.3.0)
- [touch-2.3.1](https://github.com/JarvusInnovations/sencha-hotfixes/tree/touch-2.3.1)
- [touch-2.4.0.487](https://github.com/JarvusInnovations/sencha-hotfixes/tree/touch-2.4.0.487)
- [touch-2.4.1.527](https://github.com/JarvusInnovations/sencha-hotfixes/tree/touch-2.4.1.527)
- [ext-5.0.0.736](https://github.com/JarvusInnovations/sencha-hotfixes/tree/ext-5.0.0.736)
- [ext-5.0.0.970](https://github.com/JarvusInnovations/sencha-hotfixes/tree/ext-5.0.0.970)
- [ext-5.0.1.1255](https://github.com/JarvusInnovations/sencha-hotfixes/tree/ext-5.0.1.1255)
- [ext-5.1.1.451](https://github.com/JarvusInnovations/sencha-hotfixes/tree/ext-5.1.1.451)

## Using hotfixes
This repository has separate branches for each framework+version, with the master branch serving as a template for new branches.

### Step 1) Clone a branch into your <kbd>packages</kbd> folder
Open a terminal in your app's or workspace's <kbd>packages</kbd> directory and clone the branch for the framework+version you're using into a directory called <kbd>jarvus-hotfixes</kbd>:

  `git clone -b touch-2.4.1.527 https://github.com/JarvusInnovations/sencha-hotfixes.git jarvus-hotfixes`

### Step 2) Add package to app's requirements
Open the <kbd>app.json</kbd> file in your app's directory and add `"jarvus-hotfixes"` to the array following the existing `"requires"` attribute:

```json
    "requires": [
        "jarvus-hotfixes"
    ],
```

### Step 3) Refresh bootstrap.js
In order for the overrides contained in the package to be automatically loaded by our app, the <kbd>bootstrap.js</kbd> file generated by Sencha CMD must be updated after adding a new package to the app's `"requires"` config. Run this from your app's directory:

  `sencha app refresh`


## Pull requests
Pull requests containing new or improved hotfixes are welcome! We will test and review them before incorporating into our hotfix packages
