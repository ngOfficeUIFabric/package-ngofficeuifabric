[![MIT license](https://img.shields.io/npm/l/express.svg)](https://github.com/ngOfficeUIFabric/ng-officeuifabric/blob/master/LICENSE)
[![npm version](https://badge.fury.io/js/ng-office-ui-fabric.svg)](https://badge.fury.io/js/ng-office-ui-fabric)
[![bower version](https://badge.fury.io/bo/ng-office-ui-fabric.svg)](https://github.com/ngofficefabric/package-ngofficeuifabric)
[![NuGet version](https://badge.fury.io/nu/ng-office-ui-fabric.svg)](https://badge.fury.io/nu/ng-office-ui-fabric)

This repo is for the distribution of the ngOfficeUiFabric on `npm` and `bower`. The source for this module is in the [main ngOfficeUiFabric repo](https://github.com/ngOfficeUIFabric/ng-officeuifabric). Please submit issues and pull requests against that repo.

## Installing Angular Material

You can install this package locally either with `npm` or `bower`. 

### npm

```shell
# To install latest stable release 
npm install ng-office-ui-fabric

# To install latest stable release and update package.json
npm install ng-office-ui-fabric --save

# To install from HEAD of master
npm install https://github.com/ngofficeuifabric/package-ngofficeuifabric/tarball/master

# To view all installed package 
npm list;
```

### bower

```shell
# To get the latest stable version, use bower from the command line.
bower install ng-office-ui-fabric

# To get the most recent, last committed-to-master version use:
bower install ng-office-ui-fabric#master

# To save the bower settings for future use:
bower install ng-office-ui-fabric --save

# Later, you can use easily update with:
bower update
```

> Please note that ngOfficeUiFabric requires **Angular 1.4.x** or higher & **Office UI Fabric 1.1.*** or higher.


## Using the ngOfficeUiFabric Library

Now that you have installed the ngOfficeUiFabric libraries, simply include the scripts and stylesheet in your main HTML file, in the order shown in the example below. Note that npm 
will install the files under `/node_modules/ng-office-ui-fabric/` and bower will install them 
under `/bower_components/ng-office-ui-fabric/`.

### npm

```html
<!DOCTYPE html>
<html>
<head>
  <meta name="viewport" content="initial-scale=1, maximum-scale=1, user-scalable=no" />
  <!-- add Office UI Fabric stylesheets (there are minified options too) -->
  <link rel="stylesheet" href="/node_modules/office-ui-fabric/fabric.css">
  <link rel="stylesheet" href="/node_modules/office-ui-fabric/fabric.components.css">
</head>
<body ng-app="YourApp">

  <div ng-controller="YourController">
    ..
  </div>

  <!-- add angular & ngOfficeUiFabric (there are minified options too) -->
  <script src="/node_modules/angular/angular.js"></script>
  <script src="/node_modules/ng-office-ui-fabric/ngOfficeUiFabric.js"></script>

    // Include app dependency on ngOfficeUIFabric
    angular.module('YourApp', [
        'officeuifabric.core',
        'officeuifabric.components'
      ])
      .controller('YourController', YourController);

  </script>

</body>
</html>
```

### bower

```html
<!DOCTYPE html>
<html>
<head>
  <meta name="viewport" content="initial-scale=1, maximum-scale=1, user-scalable=no" />
  <!-- add Office UI Fabric stylesheets (there are minified options too) -->
  <link rel="stylesheet" href="/bower_components/office-ui-fabric/fabric.css">
  <link rel="stylesheet" href="/bower_components/office-ui-fabric/fabric.components.css">
</head>
<body ng-app="YourApp">

  <div ng-controller="YourController">
    ..
  </div>

  <!-- add angular & ngOfficeUiFabric (there are minified options too) -->
  <script src="/bower_components/angular/angular.js"></script>
  <script src="/bower_components/ng-office-ui-fabric/ngOfficeUiFabric.js"></script>

    // Include app dependency on ngOfficeUIFabric
    angular.module('YourApp', [
        'officeuifabric.core',
        'officeuifabric.components'
      ])
      .controller('YourController', YourController);

  </script>

</body>
</html>
```