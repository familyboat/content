---
title: "Element: ariaSelected property"
short-title: ariaSelected
slug: Web/API/Element/ariaSelected
page-type: web-api-instance-property
browser-compat: api.Element.ariaSelected
---

{{APIRef("DOM")}}

The **`ariaSelected`** property of the {{domxref("Element")}} interface reflects the value of the [`aria-selected`](/en-US/docs/Web/Accessibility/ARIA/Reference/Attributes/aria-selected) attribute, which indicates the current "selected" state of elements that have a selected state.

## Value

A string with one of the following values:

- `"true"`
  - : The item is selected.
- `"false"`
  - : The item is not selected.
- `"undefined"`
  - : The item is not selectable.

## Examples

In this example the `aria-selected` attribute on the element with an ID of `tab-id` is set to "true". Using `ariaSelected` we update the value to "false".

```html
<button role="tab" aria-selected="true" aria-controls="tabpanel-id" id="tab-id">
  Tab label
</button>
```

```js
let el = document.getElementById("tab-id");
console.log(el.ariaSelected); // true
el.ariaSelected = "false";
console.log(el.ariaSelected); // false
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- [ARIA: tab role](/en-US/docs/Web/Accessibility/ARIA/Reference/Roles/tab_role)
