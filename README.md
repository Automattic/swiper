# For of the Swiper.js Repo for A8C Specific Builds

The purpose of this fork is to provide a location to house Automattic specific build scripts for the Swiper.js library.

Currently custom builds are only used by the Jetpack Carousel module. 

Using a custom build means we can shave approximately 100KB off the uncompressed library bundles.

## Creating a new build for Jetpack Carousel

 - Check out this repo 
 - Run `npm install`
 - Checkout the `jetpack-build` branch and make sure the latest release changes you need are merged into this branch, while making sure the changes to the `scripts/build-config.js` file and this ReadMe are maintained.
 - Run `npm run build:prod`
 - Copy `package/swiper-bundle.js` and `package/swiper-bundle.css` to `jetpack/projects/plugins/jetpack/modules/carousel`

 ## Todo

 - Automate this process somehow