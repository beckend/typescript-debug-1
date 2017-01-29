# typescript-debug-1
tsconfig
```json
{
  "compilerOptions": {
    "noUnusedParameters": true
  }
}
```

```js
export default (one, two, three, value, state, options) => {
  if (value % 1 !== 0) {
    return this.createError('number.round', { v: value }, state, options);
  }

  return value;
};
```

`one`, `two`, `three` is marked declared but never used.
