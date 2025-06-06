# Test Vectors for the JAM Protocol

JAM protocol version 0.6.4

## Codec

- [Codec](./codec/README.md)

## State Transition Functions

We offer two types of test vectors:

- **Tiny**: designed for quick adjustments and prototyping, with reduced
  - validators count: 6
  - cores count: 2
  - epoch period: 12
  - core assignment rotation period: 4
  - ticket attempts: 3

- **Full**: vectors with production specs
  - validators count: 1023
  - cores count: 341
  - epoch period: 600
  - core assignment rotation period: 10
  - ticket attempts: 2

### STF Output

Technically, the STF execution process does not inherently produce auxiliary
outputs beyond the success or failure result. In this context, we propose
an extension to include additional information that may be beneficial for
implementors or useful for executing other subsystems reliant on values
generated post-STF execution.

When the error or success values are not pertinent to your test vector
processing procedures, you may disregard them as necessary.

A mapping of error code semantics is provided within the ASN.1 schema for each
specific subsystem.

### Vectors

- [Accumulate](./accumulate/README.md)
- [Assurances](./assurances/README.md)
- [Authorizations](./authorizations/README.md)
- [Codec](./codec/README.md)
- [Disputes](./disputes/README.md)
- [Erasure Coding](./erasure_coding/README.md)
- [History](./history/README.md)
- [Host Function](./host_function/README.md)
- [Preimages](./preimages/README.md)
- [PVM](./pvm/README.md)
- [Reports](./reports/README.md)
- [Safrole](./safrole/README.md)
- [Shuffle](./shuffle/README.md)
- [Statistics](./statistics/README.md)
- [Trie]()
