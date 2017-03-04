[![alt text][shield-status]][link-repo] [![alt text][shield-production]][link-todo] [![alt text][shield-webc]][link-webc] ![alt text][shield-animations] [![alt text][shield-deps]][link-repo] ![alt text][shield-polymer] [![alt text][shield-license]][link-license]

_[Demo and API docs][link-webc]_

##&lt;signin-button&gt;

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
  <app-bottom-nav-item icon="abn-demo:history" label="Recent"></app-bottom-nav-item>
  <app-bottom-nav-item icon="abn-demo:favorite" label="Favorites"></app-bottom-nav-item>
  <app-bottom-nav-item icon="abn-demo:near-me" label="Nearby"></app-bottom-nav-item>
</app-bottom-nav>
```

The demo here uses icons from the file [`app-bottom-nav/demo/demo-icons.html`](https://github.com/samthecodingman/app-bottom-nav/blob/master/demo/demo-icons.html).

## Updates

**Version 0.0.1 -> Version 0.0.4**
- (Fixes Issue #1) Improved icon documentation for demo code.
- (Issue #2) Added `force-compact` property to `app-bottom-nav` element. This will force the `compact` attribute on its children which normally only happens when 4 or 5 children are present.
- (Fixes Issue #2) Added `notify` property attribute to `selected` on `app-bottom-nav` element.
- **Breaking:** `force()` renamed to `showAlways()` on `app-bottom-nav` element
- **Breaking:** `clearForce()` renamed to `showDefault()` on `app-bottom-nav` element
- **Breaking:** `toggleForce()` renamed to `toggleForceNarrow()` on `app-bottom-nav` element
- Changed deprecated `reflect` entries on properties to `reflectToAttribute` on `app-bottom-nav` element
- Removed 2 instances of `console.log` from `app-bottom-nav.html`
- Removed 1 instance of `console.log` from `animations/compact-grow-animation.html`
- Cleaned up animations for grow and shrink in `animations`
- Changed animation duration to 200ms in `app-bottom-nav-item` element
- Added ripple animation (based on `Polymer.PaperRippleBehavior`) to `app-bottom-nav-item` element
- CSS scoping bug should be fixed (in theory)
- Updated README format (added Polymer version badge, used attachments)
- Fix `bower.json` version information


## To Do List
This is a brief list of tasks that are yet to be completed. Feel free to open an issue or contribute a pull request if you think you can help.
- Implement Tests
- Prepare for Polymer 2.0 update
- Add ARIA/a11y support

Demo and API docs: [webcomponents.org][link-webc], [GitHub Pages][link-docs]

[link-docs]: https://samthecodingman.github.io/app-bottom-nav/
[link-license]: https://github.com/samthecodingman/app-bottom-nav/blob/master/LICENSE
[link-repo]: https://www.github.com/samthecodingman/app-bottom-nav
[link-todo]: https://www.github.com/samthecodingman/app-bottom-nav#to-do-list
[link-webc]: https://www.webcomponents.org/element/samthecodingman/app-bottom-nav
[shield-animations]: https://img.shields.io/badge/animations-yes-green.svg "Animations: yes"
[shield-deps]: https://img.shields.io/badge/dependencies-first--party-polymer-green.svg "Dependencies: first-party polymer"
[shield-license]: https://img.shields.io/badge/license-MIT-blue.svg "License: MIT"
[shield-polymer]: https://img.shields.io/badge/polymer%20version-1.0-yellow.svg "Polymer Version: 1.0"
[shield-production]: https://img.shields.io/badge/production--ready-no-red.svg "Production Ready: no"
[shield-status]: https://img.shields.io/badge/status-beta-yellow.svg "Status: beta"
[shield-webc]: https://img.shields.io/badge/webcomponents.org-published-blue.svg "Published on webcomponents.org"
