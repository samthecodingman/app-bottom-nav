# \<app-bottom-nav\>

[![Currently in beta](https://img.shields.io/badge/status-beta-yellow.svg)](https://www.github.com/samthecodingman/app-bottom-nav) [![Not suitable for production](https://img.shields.io/badge/production--ready-no-red.svg)](https://www.github.com/samthecodingman/app-bottom-nav#to-do-list) [![Published on webcomponents.org](https://img.shields.io/badge/webcomponents.org-published-blue.svg)](https://www.webcomponents.org/element/samthecodingman/app-bottom-nav) ![Element has animations](https://img.shields.io/badge/animations-yes-green.svg) [![Only first-party dependencies](https://img.shields.io/badge/dependencies-first--party-green.svg)](https://www.github.com/samthecodingman/app-bottom-nav#usage-instructions) [![MIT License](https://img.shields.io/badge/license-MIT-blue.svg)](https://www.github.com/samthecodingman/app-bottom-nav/LICENSE)

A [Material Design](https://material.io/guidelines/components/bottom-navigation.html) bottom navigation element.

### Usage Instructions

By default, the element will only be visible when the viewport is less than
640px. This corresponds to the default `app-drawer-layout` responsive width and
means the `app-bottom-nav` will show when the app-drawer retracts.

- Each navigation option is added as an `app-bottom-nav-item` element and assigned
an icon and a text label.
- `app-bottom-nav` should only contain between 3 and 5 `app-bottom-nav-item` elements.
- The `selected` attribute will contain the label of the currently selected navigation item.

**Dependencies:** This element is only dependent on first-party polymer elements outside of this element pack.

## Example

```html
<app-bottom-nav selected="{{selected}}">
  <app-bottom-nav-item icon="history" label="Recent"></app-bottom-nav-item>
  <app-bottom-nav-item icon="favorite" label="Favorites"></app-bottom-nav-item>
  <app-bottom-nav-item icon="maps:near-me" label="Nearby"></app-bottom-nav-item>
</app-bottom-nav>
```

## To Do List
This is a brief list of tasks that are yet to be completed. Feel free to open an issue or contribute a pull request if you think you can help.
- Implement Tests
- Fix CSS Custom Properties not scoping properly
- Add ARIA/a11y support

More information can be found on the [documentation pages](https://samthecodingman.github.io/app-bottom-nav/).
