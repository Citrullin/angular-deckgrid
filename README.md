# angular-deckgrid-filter-order
Modified Version of Deckgrid by Akoenig

With this Version you can use filter and orderBy without any problems. 

[Version 0.5.0]
I fixed the following problems:
- No attributes for filter and orderBy
- No re-rendering of the directive after changing the model of orderBy or filter

A lightweight masonry-like grid for AngularJS.

[Website / Demo](http://akoenig.github.io/angular-deckgrid)

## Installation

1. `bower install git://github.com/Citrullin/angular-deckgrid-filter-order.git
2. Include `angular-deckgrid` in your HTML.

    ```html
    <script src="<your-bower-components>/angular-deckgrid-filter-order/angular-deckgrid.js"></script>
    ```

3. Inject the `angular-deckgrid` module in your application.

    ```js
    angular.module('your.module', [
        'akoenig.deckgrid'
    ]);
    ```

## Usage

photos (Array with objects)
orderby (Orderby Model)
filter (Filter Function)

    <select ng-model="orderList">
	<option value="Price">Lower to Higher</option>
	<option value="-Price">Higher to Lower</option>
    </select>

    <div deckgrid class="deckgrid" source="photos" orderby="orderList" filter="filterList">
        <div class="a-card">
            <h1>{{card.title}}</h1>

            <img src="" data-ng-src="{{card.src}}">
        </div>
    </div>

For more information about the Usage read the [original Repository](https://github.com/akoenig/angular-deckgrid)

## Credits

* All the [people](https://github.com/akoenig/angular-deckgrid/blob/master/CONTRIBUTORS.md) who made outstanding contributions to the `angular-deckgrid` so far.
* [AngularJS](http://angularjs.org) Needless to say. You know the beast. One of the best frontend frameworks in the world.

*[Akoening](https://github.com/akoenig/angular-deckgrid) Original Deckgrid without this feature.

## Author

Philipp Blum by [jakiku](http://www.jakiku.com/de/)
