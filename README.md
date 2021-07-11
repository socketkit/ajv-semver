# ajv-semver

Adds a `semver` format to [Ajv](https://ajv.js.org).

## Install

```bash
npm i --save @socketkit/ajv-semver
```

## Setup

```javascript
import Ajv from 'ajv'
import semver from '@socketkit/ajv-semver'
const ajv = new Ajv()
semver(ajv)
```

## Usage

When defining your JSON schema, use the `format` keyword with ther value set to `semver`. For example

```json
{
  "type": "object",
  "properties": {
    "semver": {
      "type": "string",
      "format": "semver"
    }
  }
}
```
