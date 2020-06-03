# WPML Installer

## Usage

Add a repository for each WPML plugin you want to use (under repositories in composer.json)

```json
{
  "type": "package",
  "package": {
    "name": "wpml/wpml-multilingual-cms",
    "version": "4.3.15",
    "type": "wordpress-plugin",
    "dist": {
      "type": "zip",
      "url": "https://httpbin.org/status/400?"
    },
    "require": {
      "enelogic/wpml-installer": "^0.1",
      "composer/installers": "^1.0"
    }
  }
}
```

(trailing slash matters on that httpbin url)

And then require:

```sh
composer require wpml/wpml-multilingual-cms
```

or in composer.json, add this to require

```json
"wpml/wpml-multilingual-cms": "*",
```

Then set up environment vars for:

`WPML_KEY` = subscription_id parameter on the url
`WPML_USER_ID` = user_id parameter on the url

You can find these by logging into WPML website and copy/pasting a download link for any of the plugins.

You should be all set - rinse and repeat for other WPML plugins - a fuller config is below for easier copy/paste.

## More packages for easy copy/paste - edit the versions to whatever is current.

```json
({
  "type": "package",
  "package": {
    "name": "wpml/wpml-multilingual-cms",
    "version": "4.3.15",
    "type": "wordpress-plugin",
    "dist": {
      "type": "zip",
      "url": "https://httpbin.org/status/400?"
    },
    "require": {
      "enelogic/wpml-installer": "^0.1",
      "composer/installers": "^1.0"
    }
  }
},
{
  "type": "package",
  "package": {
    "name": "wpml/wpml-string-translation",
    "version": "3.0.11",
    "type": "wordpress-plugin",
    "dist": {
      "type": "zip",
      "url": "https://httpbin.org/status/400?"
    },
    "require": {
      "enelogic/wpml-installer": "^0.1",
      "composer/installers": "^1.0"
    }
  }
},
{
  "type": "package",
  "package": {
    "name": "wpml/wpml-translation-management",
    "version": "2.9.8",
    "type": "wordpress-plugin",
    "dist": {
      "type": "zip",
      "url": "https://httpbin.org/status/400?"
    },
    "require": {
      "enelogic/wpml-installer": "^0.1",
      "composer/installers": "^1.0"
    }
  }
},
{
  "type": "package",
  "package": {
    "name": "wpml/wpml-sticky-links",
    "version": "1.5.2",
    "type": "wordpress-plugin",
    "dist": {
      "type": "zip",
      "url": "https://httpbin.org/status/400?"
    },
    "require": {
      "enelogic/wpml-installer": "^0.1",
      "composer/installers": "^1.0"
    }
  }
},
{
  "type": "package",
  "package": {
    "name": "wpml/wpml-cms-nav",
    "version": "1.5.2",
    "type": "wordpress-plugin",
    "dist": {
      "type": "zip",
      "url": "https://httpbin.org/status/400?"
    },
    "require": {
      "enelogic/wpml-installer": "^0.1",
      "composer/installers": "^1.0"
    }
  }
},
{
  "type": "package",
  "package": {
    "name": "wpml/wpml-media",
    "version": "2.5.5",
    "type": "wordpress-plugin",
    "dist": {
      "type": "zip",
      "url": "https://httpbin.org/status/400?"
    },
    "require": {
      "enelogic/wpml-installer": "^0.1",
      "composer/installers": "^1.0"
    }
  }
})
```

and require:

```json
"wpml/wpml-multilingual-cms": "*",
"wpml/wpml-string-translation": "*",
"wpml/wpml-translation-management": "*",
"wpml/wpml-sticky-links": "*",
"wpml/wpml-cms-nav": "*",
"wpml/wpml-media": "*",
```
