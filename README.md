# Licence-Sorter

This CLI takes a JSON file outputted from the NPM library [license-checker](https://www.npmjs.com/package/license-checker) and sorts it so that the results are grouped by their licenses.
<br />
### Eg.
<img src="https://tobysmith568.github.io/License-Sorter/before-and-after-labelled.png" />
<br />

## Installation and Usage (CLI)
```
$ npm install license-sorter -g

$ license-sorter --input licenses.json --output licenses-sorted.json
```
- Input: The file to be converted
- Output: The file to be created

If either flag is omitted the CLI will prompt you for the inputs.

## Installation and Usage (Programmatic use)
```
$ npm install license-sorter
```
```js
const licenseSorter = require("license-sorter");

licenseSorter.convertFile("licenses.json", "licenses-sorted.json")
.then(() => {

})
.catch(() => {

});
```
```ts
import * as licenseSorter from "license-sorter";

await licenseSorter.convertFile("licenses.json", "licenses-sorted.json");
```

This library is in no way affiliated with [license-checker](https://www.npmjs.com/package/license-checker).
