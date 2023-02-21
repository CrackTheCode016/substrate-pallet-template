License: Unlicense

# Substrate Pallet Template

Contains a blank, clean pallet ready for hacking. Taken from its source - [the Substrate Node Template](https://github.com/substrate-developer-hub/substrate-node-template).

A pallet works like any other cargo crate - meaning you can incoprorate it into a Substrate node instance by adding it to `runtime/Cargo.toml`:

```toml
pallet-<name> = { version = "4.0.0-dev", default-features = false, git = "github-link-to-your-pallet", branch = "<branch-name-usually-main>" }
```

Or, you could build a whole library of pallets, similar to [FRAME](https://github.com/paritytech/substrate/tree/master/frame).

## Building 

```
cargo build
```

## Testing
```
cargo test
```

With benchmarks: 

```
cargo test --features runtime-benchmarks 
```