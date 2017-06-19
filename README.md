
# Covenant Favicon Generator

Easily regenerate the favicon assets for [Covenant](http://www.covenantclassicalschool.org)

## Generate the favicon assets

The icons are all generated using the master [faviconMaster.png](assets/faviconMaster.png) image.

From the command line, run:

```sh
npm install
```

Then, generate the favicons into the [dist](dist) directory:

```sh
npm run generate
```

Update the favicon data script (in case the file format was changed):

```sh
npm run update
```

**NOTE**: The assets directory also contains some logo files that get copied to the dist folder on 'generate':

- [logo.png](assets/logo.png): Standard logo (480 x 480)

### Config

Refer to the [realfavicongenerator.net api documentation](http://realfavicongenerator.net/api/), and modify 
the [faviconDescription.json](faviconDescription.json) file accordingly.

## Deploy the favicons to the site

Inspect the [dist/index.html](dist/index.html) file `<head>` tags to copy into the site's html as needed.
Copy all other assets from the dist directory to the root of the site.
