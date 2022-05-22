# hash-rs

> Forked from [Gankra/hash-rs](https://github.com/Gankra/hash-rs) to add more hashes.

To view the results, clone this repository, run `node index.js` and go to [localhost:8082](http://localhost:8082).

To build the results, run `cargo run` (this will in turn run Cargo bench in the background).
This will produce some csv's that index.html will consume.

Currently Sip, Fx, Fnv, XXH3 (`twox_hash`, `xxhash-rust`), XXHash64, HighwayHash, and SeaHash are supported. Other hasher crates were in an inappropriate state.
Patches to change this welcome!

This does not necessarily reflect the quality of the algorithms themselves, but rather the performance
of the implementations when used with Rust's hasher infrastructure.

I would like to bench different workloads in the future (everything has been set up to enable this generically).
