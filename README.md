# vindex-sigstore (Experimental)

`vindex-sigstore` packages the [Verifiable Index (`vindexd`)](https://github.com/transparency-dev/incubator/tree/main/vindex) daemon and Sigstore's Rekor Identity Monitor WebAssembly mapping functions (`mapper-hashedrekord.wasm` and `mapper-identity.wasm`) as independent, separately verifiable artifacts.

## Building Locally

```bash
# Build bin/vindexd
make all

# Generate an Ed25519 Note signing and verification keypair for the Output Log
make keygen
# Or specify a custom origin:
make keygen ORIGIN=my.vindex.org

# Coming soon: generating ML-DSA keypairs

# Build Docker images (vindexd)
make docker-build
```
