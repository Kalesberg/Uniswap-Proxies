# Proxies

Smart contracts for upgradeable proxies.


If you deploy a new version of `DelegateCallProxyManager.sol` without using the artifact in /artifacts (handled automatically by buidler), your local build may result in different bytecode. If that happens, the code hashes in `CodeHashes.sol` will be incorrect and the proxy address derivation functions will not work. Either use the already built artifacts in the package or replace the codehashes with the new values. See: [script for generating the CodeHashes contract](./scripts/write-code-hashes.js)

## Test

```
npm run test
```
