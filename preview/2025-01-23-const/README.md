## 2025-01-23 Cardano Constitution to Replace the Interim Constitution

### On-Chain Details

- Transaction:

- Metadata Anchor Hash (`blake2b-256`): `8b9131c3efe52c747fda90d38930231b3a771ec7e22173ffd37ff42283f1bb18`
- Metadata Anchor URI: <https://raw.githubusercontent.com/IntersectMBO/governance-actions/refs/heads/main/preview/2025-01-23-const/metadata.jsonld>

### Details

- [JSON Document](./metadata.jsonld)
- [Rendered Human Readable Markdown](./metadata.jsonld.md)

### Action Files

Provided in this directory are the `cardano-cli` governance action file which will be submitted:

- [New Constitution Action File](./)
- [Action file JSON (human readable)](./)

### Verification

It is recommended that third parties audit and verify the contents of this directory.

#### Check hash

Using `cardano-cli` (without cloning).

```shell
cardano-cli hash anchor-data --url https://raw.githubusercontent.com/IntersectMBO/governance-actions/refs/heads/main/preview/2025-01-23-const/metadata.jsonld
```

Using `b2sum` (without cloning).

```shell
curl -s https://raw.githubusercontent.com/IntersectMBO/governance-actions/refs/heads/main/preview/2025-01-23-const/metadata.jsonld | b2sum -l 256
```

#### Check action file

#### Check JSON

Ensure the provided action file JSON is representative of the action.

Using `cardano-cli`.

```shell
cardano-cli conway governance action view --action-file <(curl -s https://raw.githubusercontent.com/IntersectMBO/governance-actions/refs/heads/main/preview/2024-12-19-conts/XXXX.action)
```

#### Inspect values

1. Ensure the `anchor` values are as expected - matching the values in this repo.

2. Ensure `governance action` type is as expected, and has the on-chain effect intended - as described by the metadata in this repo.

3. Ensure `return address` is for the correct network, registered and expected.
