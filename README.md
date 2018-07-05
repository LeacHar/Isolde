# SortableJs

> Project is WIP, it's not advisable to use it for professionnal project.

Sortable is a javascript plugin allow you to reorganize elements from a "masonry" grid.
## Quick start
> ### Install
> This package cannot be installed with npm/yarn yet.
> <br>
> Waiting for a stable version.

### Load
**Static HTML**

> The next major version expect to use a css file for animations 

Put the script at the bottom of your markup:

```js
<script src="[YOUR_PATH]/sortablejs.min.js"></script>
```

### Usage
1. Create links (a) that have the attribute `data-sjslink` with an identification value corresponding to a family (ex: food, development, etc.).
2. Wrap your items (div, a, img, span, li etc.) with an item element (div, ul etc.) that have the attribute `data-sjsel` with an identification value corresponding to his family.
3. Wrap your items (div, a, img, span, li etc.) with a container element (div, ul etc.) that have the attribute `id="sortable"`.


```html
<!-- 1st step -->
<ul>
    <li>
        <a data-sjslink="food">
            [...]
        </a>
    </li>
    <li>
        <a data-sjslink="development">
            [...]
        </a>
    </li>
</ul>

<!-- 3st step -->
<div id="sortable">

    <!-- 2nd step -->
    <div data-sjsel="food"> [...] </div>
    <div data-sjsel="development"> [...] </div>
    <div data-sjsel="development"> [...] </div>
</div>
```

Call the plugin function and it's work !

```js
<script type="text/javascript">
    var sortable = new Sortable();
</script>
```

## Documentation
Please read [OPTIONS.md](https://github.com/TristanBlg/sortableJs/blob/master/docs/OPTIONS.md).
