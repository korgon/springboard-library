# Slideout Module

The module adds the ability to compare products. Fields must be marked as 'compare' in the SMC.

|Option|Description|
|------|-----------|
|no options| - |

```js
this.importer.include('compare');
```

---

### Template Targets

To add the compare button, add the following target to your product display template (once for each product):

```html
<div class="searchspring-compare-button"></div>
```

To attach the compare box, add this target (this should exist only once):

```html
<div ng-if="compare.active && !compare.open" class="searchspring-compare-box"></div>
```

The compare modal window will target need this target added (should exist once):
```html
<div ng-if="compare.open && compare.results.length >= 2" id="searchspring-compare"></div>
```
