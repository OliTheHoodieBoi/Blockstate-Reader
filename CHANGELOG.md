# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## Upcoming

### Added

- [IMP documentation](https://github.com/Arcensoth/imp-spec/blob/master/docs/imp_doc.md).
- Reading of NBT data from block.
- Block tags for blocks with/without NBT data.
- Reading of block id.

### Changed

- Read output location moved from storage `blockstate:data read` to `blockstate:output Properties`.
- Moved block tags for [properties](https://github.com/OliTheHoodieBoi/Blockstate-Reader#Properties) to `#blockstate:property/*`.
- `resources` migrated to [mcblockstates](https://github.com/OliTheHoodieBoi/mcblockstates)
- New and improved README.
- Improved performance.

### Fixed

- Missing property `conditional`.

## 1.0.0

### Added

- Ability to read [properties](https://github.com/OliTheHoodieBoi/Blockstate-Reader#Properties) to storage.
- Block tags for [properties](https://github.com/OliTheHoodieBoi/Blockstate-Reader#Properties).
