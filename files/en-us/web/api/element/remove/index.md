---
title: "Element: remove() method"
short-title: remove()
slug: Web/API/Element/remove
page-type: web-api-instance-method
browser-compat: api.Element.remove
---

{{APIRef("DOM")}}

The **`Element.remove()`** method removes the element from its parent node.
If it has no parent node, calling `remove()` does nothing.

## Syntax

```js-nolint
remove()
```

### Parameters

None.

### Return value

None ({{jsxref("undefined")}}).

## Examples

### Using `remove()`

```html
<div id="div-01">Here is div-01</div>
<div id="div-02">Here is div-02</div>
<div id="div-03">Here is div-03</div>
```

```js
const element = document.getElementById("div-02");
element.remove(); // Removes the div with the 'div-02' id
```

### `Element.remove()` is unscopable

The `remove()` method is not scoped into the `with` statement.
See {{jsxref("Symbol.unscopables")}} for more information.

```js
with (node) {
  remove();
}
// ReferenceError: remove is not defined
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- {{domxref("CharacterData.remove()")}}
- {{domxref("DocumentType.remove()")}}
