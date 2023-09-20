# Vasku keys

![cover](docs/cover.svg)

Use key pair in [Vasku](https://github.com/kokkekpek/vasku) scripts

![npm](https://img.shields.io/npm/v/vasku-keys?label=npm)
![downloads](https://img.shields.io/npm/dt/vasku-keys?label=downloads)

## Read key pair from JSON file

```typescript
import { readKeys } from 'vasku-keys'
// ...
const keys: KeyPair = readKeys('/home/user/keys/GiverV2.keys.json')
```

## Generate random key pair if key file does not exist

```typescript
import { generateOrReadKeys } from 'vasku-keys'
// ...
const keys: KeyPair = await generateOrReadKeys('/home/user/keys/GiverV3.keys.json')
```

## Generate JSON file with random key pair in keys directory if key file does not exist

```typescript
import { namedKeys } from 'vasku-keys'
// ...
const keys: KeyPair = await namedKeys('giver')
```

## Development

[CONTRIBUTING.md](./CONTRIBUTING.md)