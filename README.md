# Vendee keys

![cover](docs/cover.svg)

Methods of working with key pair in [Vendee](https://github.com/kokkekpek/vendee) scripts and tests

![npm](https://img.shields.io/npm/v/vendee-keys?label=npm)
![downloads](https://img.shields.io/npm/dt/vendee-keys?label=downloads)

## How to use

### Read key pair from JSON file

```typescript
import { readKeys } from 'vendee-keys'
// ...
const keys: KeyPair = readKeys('/home/user/keys/GiverV2.keys.json')
```

### Generate random key pair if key file does not exist

```typescript
import { generateOrReadKeys } from 'vendee-keys'
// ...
const keys: KeyPair = await generateOrReadKeys('/home/user/keys/GiverV3.keys.json')
```

### Generate JSON file with random key pair in keys directory if key file does not exist

```typescript
import { namedKeys } from 'vendee-keys'
// ...
const keys: KeyPair = await namedKeys('giver')
```

## Development

### Build

```shell
yarn build
```

### Remove build directory

```shell
yarn clean
```

### Lint

Run before commit

```shell
yarn lint
```

```shell
yarn fix
```