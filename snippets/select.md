### select

Retrieve a property that indicated by the selector from object.

If property not exists returns `undefined`.

```js
const select = (from, selector) =>
  selector.split('.').reduce((prev, cur) => prev && prev[cur], from);

// const obj = {selector: {to: {val: 'val to select'}}};
// select(obj, 'selector.to.val'); -> 'val to select'
```
