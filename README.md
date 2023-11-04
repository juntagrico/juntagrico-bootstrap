# juntagrico-bootstrap
bootstrap source with juntagrico configurations

## Setup

1. install npm on your system
2. install and update packages
    ```
    npm install
    ```

## Build & Save

1. compile css
    ```
    npm run dist
    ```
2. copy files from `dist/css` to `juntagrico/static/external/bootstrap-x.x.x/css` in the juntagrico project 
3. commit and push changes

## Modify Bootstrap

1. make adjustments in the `juntagrico_*.scss`-files
2. rebuild

## Upgrade Bootstrap

1. download Bootstrap source code of desired version
2. copy scss folder into this project
3. copy `build/postcss.config.js` into this project
4. in `package.json` update `version` to match the bootstrap version (for consistency)
5. in `package.json` update the versions under `devDependencies` to match the versions from the `package.json` in the Bootstrap source code
6. update packages
    ```
    npm update
    ```
