Wayne State Style Guide
=========

Wayne State University global header/footer and other general styles. Build on [Bootstrap 3.3.x](https://getbootstrap.com/).

## Desktop
![desktop](http://waynestate.github.io/styleguide/images/header-fd5-desktop.png "Header on the desktop")

## Tablet
![tablet](http://waynestate.github.io/styleguide/images/header-fd5-tablet.png "Header on the tablet")

## Mobile
![mobile](http://waynestate.github.io/styleguide/images/header-fd5-mobile.png "Header on the mobile")

Compile with Bootstrap 3.3.x
=========

Install the latest bootstrap-sass npm package

```
npm install bootstrap-sass --save-dev
npm install git://github.com/waynestate/styleguide.git#feature/bootstrap3 --save-dev
```

Add bootstrap and the wsuheader styles in the app stylesheet

```
// Framework
@import "partials/vars";
@import "node_modules/bootstrap-sass/assets/stylesheets/bootstrap";

// University specific
@import "node_modules/@waynestate/styleguide/src/scss/wsuheader";

// Site specific
...
```

Copy the blade templates into the `views` directory

```
mkdir -p app/resources/views/partials/
cp node_modules/@waynestate/styleguide/src/blade/*.blade.php app/resources/views/partials/
```

Include the blade templates in the view

```
<body>

@include('partials.header')
...

@include('partials.footer')
</body>
```
