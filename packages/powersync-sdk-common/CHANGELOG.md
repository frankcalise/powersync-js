# @journeyapps/powersync-sdk-common

## 0.1.0

### Minor Changes

- 210de9d: Bump version for Beta release

## 0.0.2

### Patch Changes

- ca458d3: Updated logic to correspond with React Native Quick SQLite concurrent transactions. Added helper methods on transaction contexts.

  API changes include:

  - Removal of synchronous DB operations in transactions: `execute`, `commit`, `rollback` are now async functions. `executeAsync`, `commitAsync` and `rollbackAsync` have been removed.
  - Transaction contexts now have `get`, `getAll` and `getOptional` helpers.
  - Added a default lock timeout of 2 minutes to aide with potential recursive lock/transaction requests.

- b125f75: Use default timeout in post streaming warning message. Update connectivity status on streaming messages.
- ab9957b: Fix update trigger for local only watched tables.
- 413a4d0: Added better logging of streaming errors. Added warnings if Polyfills are not correctly configured.

## 0.0.1

### Patch Changes

- aad52c8: Updated watched queries to trigger for local only tables.
- 822bab9: Bump version to exit prerelease mode. Update SDK readme with known issues.

## 0.0.1-alpha.1

### Patch Changes

- aad52c8: Updated watched queries to trigger for local only tables.