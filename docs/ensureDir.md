# ensureDir(dir, callback)

Ensures that the directory exists. If the directory structure does not exist, it is created. Like `mkdir -p`.

**Aliases:** `mkdirs()`, `mkdirp()`

**Sync:** `ensureDirSync()`, `mkdirsSync()`, `mkdirpSync()`

## Example:

```js
const fs = require('fs-extra')

const dir = '/tmp/this/path/does/not/exist'
fs.ensureDir(dir, err => {
  console.log(err) // => null
  // dir has now been created, including the directory it is to be placed in
})
```
