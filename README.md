vscode-js-template-tag
====================

Adds JavaScript syntax highlighting for JavaScript template literals like `js\`1+1\``.

## Match on 

```js
javascript`` | js`` | typescript`` | ts`` | jsx`` | tsx``
```

## Example

```js
const code = ts`
  const truthy = (val: any): boolean => !!val;
`;
```

## Caveat

You are responsible for defining the template literal yourself -- this extension just adds syntax highlighting for it. If you don't need any custom processing, you can use `String.raw`:

```js
const js = String.raw;
const ts = String.raw;

// later

js`1 + 1`;
```