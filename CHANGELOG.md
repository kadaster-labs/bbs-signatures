# [1.1.0](https://github.com/mattrglobal/bbs-signatures/compare/1.0.0...1.1.0) (2022-07-11)

# [1.0.0](https://github.com/mattrglobal/bbs-signatures/compare/0.7.0...1.0.0) (2022-01-09)

# [0.7.0](https://github.com/mattrglobal/bbs-signatures/compare/0.6.0...0.7.0) (2021-12-08)

### Bug Fixes

- strict check for given messages count and originally revealed ([fd1fbbf](https://github.com/mattrglobal/bbs-signatures/commit/fd1fbbfd4ac31a2c77e113ff611c6abc81851605))

# [0.6.0](https://github.com/mattrglobal/bbs-signatures/compare/0.5.0...0.6.0) (2021-05-25)

BREAKING CHANGES: Support for asm.js has been removed due to its poor performance and it creating bloat for all
package consumers. Support for NodeJS 10 which is now EOL has also been removed due in-compatibility with TextEncoder/TextDecoder that is used in the translated ES module generated by wasm-pack.

### Bug Fixes

- handle when no. of message out of bound ([c3375a4](https://github.com/mattrglobal/bbs-signatures/commit/c3375a40f634ee317e4d5910649c4d8cb372daf4))
- verify proof bug ([#85](https://github.com/mattrglobal/bbs-signatures/issues/85)) ([ec016ef](https://github.com/mattrglobal/bbs-signatures/commit/ec016efdd5d412c4a9dea5470c4295297394f2b2))

### Features

- update approach to generating wasm ([#84](https://github.com/mattrglobal/bbs-signatures/issues/84)) ([f1afe8b](https://github.com/mattrglobal/bbs-signatures/commit/f1afe8be1fa69831f983d65908d132ef407d244b))

# [0.5.0](https://github.com/mattrglobal/bbs-signatures/compare/0.3.0...0.5.0) (2021-02-23)

BREAKING CHANGES: The API exposed by this library is now promise based see [#61](https://github.com/mattrglobal/bbs-signatures/issues/61) for more details.

### Bug Fixes

- set private key as defined on generate returntype ([#47](https://github.com/mattrglobal/bbs-signatures/issues/47)) ([5b29ec8](https://github.com/mattrglobal/bbs-signatures/commit/5b29ec86754e085f6db4dac4409f409da0990e1e))
- **sample:** update references to generateBls12381G2KeyPair ([#48](https://github.com/mattrglobal/bbs-signatures/issues/48)) ([691fe74](https://github.com/mattrglobal/bbs-signatures/commit/691fe7491664e5a1196eab08f2066fbd8996cd16))
- **sample:** use byte arrays instead of strings ([#51](https://github.com/mattrglobal/bbs-signatures/issues/51)) ([fcb06c9](https://github.com/mattrglobal/bbs-signatures/commit/fcb06c927d696f43453ec93aad11444d06d32cd3)), closes [#49](https://github.com/mattrglobal/bbs-signatures/issues/49)

### Features

- change to use byte arrays for messages and support generating g1 keys ([#40](https://github.com/mattrglobal/bbs-signatures/issues/40)) ([92238cf](https://github.com/mattrglobal/bbs-signatures/commit/92238cf0895cde7a88c2ce6a830bf07bf2a7d28d))
- **sample:** update to the latest released version 0.4.0 ([f8fa318](https://github.com/mattrglobal/bbs-signatures/commit/f8fa3185787e2edb1484d942bd83a86d42f9a05f)), closes [#50](https://github.com/mattrglobal/bbs-signatures/issues/50) [#50](https://github.com/mattrglobal/bbs-signatures/issues/50) [#49](https://github.com/mattrglobal/bbs-signatures/issues/49)
- migrate to async based api ([#61](https://github.com/mattrglobal/bbs-signatures/issues/61)) ([5dbd924](https://github.com/mattrglobal/bbs-signatures/commit/5dbd924fe601b8d085d80b68b0b69b1e7b892022))

# [0.4.0](https://github.com/mattrglobal/bbs-signatures/compare/0.3.0...0.4.0) (2020-08-27)

### Bug Fixes

- uint8array return type casting ([#32](https://github.com/mattrglobal/bbs-signatures/issues/32)) ([28ed2fa](https://github.com/mattrglobal/bbs-signatures/commit/28ed2fa998562b253b1e793ff35d773602a88027))

### Features

- add asm.js roll back support ([#30](https://github.com/mattrglobal/bbs-signatures/issues/30)) ([4d28ad3](https://github.com/mattrglobal/bbs-signatures/commit/4d28ad3bce39e207a04ef660d478983212abde6c))
- add node bbs roll back support ([#33](https://github.com/mattrglobal/bbs-signatures/issues/33)) ([49aee81](https://github.com/mattrglobal/bbs-signatures/commit/49aee811ca73854456e9404b384a4935063f8e0a))
- change to use byte arrays for messages and support generating g1 keys ([#40](https://github.com/mattrglobal/bbs-signatures/issues/40)) ([92238cf](https://github.com/mattrglobal/bbs-signatures/commit/92238cf0895cde7a88c2ce6a830bf07bf2a7d28d))

### BREAKING CHANGES

- generateBls12381KeyPair has been changed to generateBls12381G2KeyPair
- All operations involving messages and nonces are now in terms of Uint8Array's rather than strings

# [0.3.0](https://github.com/mattrglobal/bbs-signatures/compare/0.2.0...0.3.0) (2020-07-20)

### Bug Fixes

- uint8array return type casting ([#32](https://github.com/mattrglobal/bbs-signatures/issues/32)) ([28ed2fa](https://github.com/mattrglobal/bbs-signatures/commit/28ed2fa998562b253b1e793ff35d773602a88027))

### Features

- add asm.js roll back support ([#30](https://github.com/mattrglobal/bbs-signatures/issues/30)) ([4d28ad3](https://github.com/mattrglobal/bbs-signatures/commit/4d28ad3bce39e207a04ef660d478983212abde6c))
- add node bbs roll back support ([#33](https://github.com/mattrglobal/bbs-signatures/issues/33)) ([49aee81](https://github.com/mattrglobal/bbs-signatures/commit/49aee811ca73854456e9404b384a4935063f8e0a))

# [0.2.0](https://github.com/mattrglobal/bbs-signatures/compare/v0.1.0...0.2.0) (2020-06-04)

### Features

- add browser sample ([#27](https://github.com/mattrglobal/bbs-signatures/issues/27)) ([fdec4fc](https://github.com/mattrglobal/bbs-signatures/commit/fdec4fcf6645b7b94a704fc5fab1fa5d74c19d01))
- add node.js sample ([#25](https://github.com/mattrglobal/bbs-signatures/issues/25)) ([04042c2](https://github.com/mattrglobal/bbs-signatures/commit/04042c247689ebf5ba78ebd970c2c666fda34fa6))

# 0.1.0 (2020-06-04)

Initial release
