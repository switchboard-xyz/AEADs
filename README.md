# RustCrypto: Authenticated Encryption with Associated Data
[![Build Status](https://travis-ci.org/RustCrypto/AEADs.svg?branch=master)](https://travis-ci.org/RustCrypto/AEADs) [![dependency status](https://deps.rs/repo/github/RustCrypto/AEADs/status.svg)](https://deps.rs/repo/github/RustCrypto/AEADs)

Collection of [Authenticated Encryption with Associated Data (AEAD)][1]
algorithms written in pure Rust.

## Warnings

Crates in this repository have not yet received any formal cryptographic and
security reviews.

**USE AT YOUR OWN RISK.**

## Usage

Crates functionality is expressed in terms of traits defined in the [`aead`][2]
crate.

## Crates
| Name | Crates.io | Documentation |
| ---- | :--------:| :------------:|
| [AES-GCM](https://en.wikipedia.org/wiki/Galois/Counter_Mode) | [![crates.io](https://img.shields.io/crates/v/aes-gcm.svg)](https://crates.io/crates/aes-gcm) | [![Documentation](https://docs.rs/aes-gcm/badge.svg)](https://docs.rs/aes-gcm) |
| [AES-GCM-SIV](https://en.wikipedia.org/wiki/AES-GCM-SIV) | [![crates.io](https://img.shields.io/crates/v/aes-gcm-siv.svg)](https://crates.io/crates/aes-gcm-siv) | [![Documentation](https://docs.rs/aes-gcm-siv/badge.svg)](https://docs.rs/aes-gcm-siv) |
| [AES-SIV](https://github.com/miscreant/meta/wiki/AES-SIV) | [![crates.io](https://img.shields.io/crates/v/aes-siv.svg)](https://crates.io/crates/aes-siv) | [![Documentation](https://docs.rs/aes-siv/badge.svg)](https://docs.rs/aes-siv) |
| [ChaCha20Poly1305](https://tools.ietf.org/html/rfc8439) | [![crates.io](https://img.shields.io/crates/v/chacha20poly1305.svg)](https://crates.io/crates/chacha20poly1305) | [![Documentation](https://docs.rs/chacha20poly1305/badge.svg)](https://docs.rs/chacha20poly1305) |
| [XSalsa20Poly1305](https://nacl.cr.yp.to/secretbox.html) | [![crates.io](https://img.shields.io/crates/v/xsalsa20poly1305.svg)](https://crates.io/crates/xsalsa20poly1305) | [![Documentation](https://docs.rs/xsalsa20poly1305/badge.svg)](https://docs.rs/xsalsa20poly1305) |

NOTE: the [`aes-ccm`][3] crate also implements the [`aead`][2] traits
used by all of the other crates in this repository.

### Minimum Supported Rust Version
All crates in this repository support Rust 1.37 or higher. In future minimum
supported Rust version can be changed, but it will be done with the minor
version bump.

## License

All crates licensed under either of

 * [Apache License, Version 2.0](http://www.apache.org/licenses/LICENSE-2.0)
 * [MIT license](http://opensource.org/licenses/MIT)

at your option.

### Contribution

Unless you explicitly state otherwise, any contribution intentionally submitted
for inclusion in the work by you, as defined in the Apache-2.0 license, shall be
dual licensed as above, without any additional terms or conditions.

[1]: https://en.wikipedia.org/wiki/Authenticated_encryption
[2]: https://docs.rs/aead
[3]: https://crates.io/crates/aes-ccm
