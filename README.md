# npmdoc-react-sortablejs

#### api documentation for  [react-sortablejs (v1.3.3)](https://github.com/cheton/react-sortable)  [![npm package](https://img.shields.io/npm/v/npmdoc-react-sortablejs.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-react-sortablejs) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-react-sortablejs.svg)](https://travis-ci.org/npmdoc/node-npmdoc-react-sortablejs)

#### A React component built on top of Sortable (https://github.com/RubaXa/Sortable).

[![NPM](https://nodei.co/npm/react-sortablejs.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/react-sortablejs)

- [https://npmdoc.github.io/node-npmdoc-react-sortablejs/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-react-sortablejs/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-react-sortablejs/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-react-sortablejs/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-react-sortablejs/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-react-sortablejs/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "name": "react-sortablejs",
    "version": "1.3.3",
    "description": "A React component built on top of Sortable (https://github.com/RubaXa/Sortable).",
    "main": "lib/index.js",
    "scripts": {
        "prepublish": "npm run lint && npm test && npm run build && npm run dist && npm run build-examples && npm run release",
        "build": "babel --out-dir ./lib ./src",
        "build-examples": "cd examples; webpack",
        "dist": "webpack; BUILD_ENV=dist webpack",
        "release": "mkdir -p releases; cp -f dist/react-sortable.js releases/react-sortable-${npm_package_version}.js; cp -f dist/react-sortable.min.js releases/react-sortable-${npm_package_version}.min.js",
        "lint": "eslint ./src",
        "lint:fix": "eslint --fix ./src",
        "precommit-check": "npm run lint",
        "test": "./babel-tap --coverage test/*.js",
        "coveralls": "./babel-tap --coverage --coverage-report=text-lcov test/*.js | node_modules/.bin/coveralls",
        "dev": "cd examples; webpack-dev-server --hot --inline --host 0.0.0.0 --port 8000 --content-base ../docs"
    },
    "pre-commit": [
        "precommit-check"
    ],
    "repository": {
        "type": "git",
        "url": "git+https://github.com/cheton/react-sortable.git"
    },
    "author": "Cheton Wu <cheton@gmail.com>",
    "license": "MIT",
    "bugs": {
        "url": "https://github.com/cheton/react-sortable/issues"
    },
    "homepage": "https://github.com/cheton/react-sortable",
    "keywords": [
        "react",
        "react-component",
        "sortable",
        "reorder",
        "drag",
        "mixin"
    ],
    "peerDependencies": {
        "react": "^0.14.0 || ^15.0.0",
        "react-dom": "^0.14.0 || ^15.0.0",
        "sortablejs": "^1.5.1"
    },
    "dependencies": {
        "prop-types": "^15.5.8"
    },
    "devDependencies": {
        "babel-cli": "^6.24.1",
        "babel-core": "^6.24.1",
        "babel-eslint": "^7.2.2",
        "babel-loader": "^6.4.1",
        "babel-plugin-transform-decorators-legacy": "^1.3.4",
        "babel-preset-es2015": "^6.24.1",
        "babel-preset-react": "^6.24.1",
        "babel-preset-stage-0": "^6.24.1",
        "coveralls": "^2.13.0",
        "eslint": "~3.19.0",
        "eslint-config-trendmicro": "~0.5.1",
        "eslint-loader": "~1.7.1",
        "eslint-plugin-import": "~2.2.0",
        "eslint-plugin-jsx-a11y": "~2.2.3",
        "eslint-plugin-react": "~6.10.3",
        "lodash": "^4.17.4",
        "nib": "^1.1.2",
        "react": "^15.5.4",
        "react-dom": "^15.5.4",
        "sortablejs": "^1.5.1",
        "stylus": "^0.54.5",
        "stylus-loader": "^3.0.1",
        "tap": "^10.3.2",
        "webpack": "^2.4.1",
        "webpack-dev-server": "^2.4.2",
        "which": "~1.2.14"
    }
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
