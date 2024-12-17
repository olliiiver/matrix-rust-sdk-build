# Test rust SDK build

Test to build the rust SDK on aarch64-apple-ios, see

https://github.com/BLAKE3-team/BLAKE3/issues/437

Which (currently) only works by disabling the NEON feature

````
export CARGO_FEATURE_NO_NEON=1
cargo build --verbose --verbose --target aarch64-apple-ios
````
