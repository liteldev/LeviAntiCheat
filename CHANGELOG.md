# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [0.4.5] - 2025-02-13

### Fixed

- Fixed NoPacket detection when server thread is blocked
- Fixed some functions not working after reloading configuration

## [0.4.4] - 2025-02-12

### Added

- Added mute/unmute command
- Added `reachDistance` and `reachDistanceCreative` in configuration file

### Changed

- Optimized command player parameter

### Fixed

- Fixed command spam in console
- Fixed AntiXray nullptr error
- Fixed AntiBadPacket [#25]
- Fixed attack related detection not working since 0.4.0

## [0.4.3] - 2025-02-11

### Added

- Added SusClientEvent

## [0.4.2] - 2025-02-10

### Added

- Added AntiSuspiciousClient

## [0.4.1] - 2025-02-04

### Changed

- Disabled anti bad packet by default

### Fixed

- Fixed anti xray obfuscation crash

## [0.4.0] - 2025-01-25

### Changed

- Support LeviLamina 1.0.0

## [0.4.0-rc.11] - 2025-01-20

### Fixed

- Fix ban command default parameter

## [0.4.0-rc.10] - 2025-01-20

### Fixed

- Fix PlayerCheatEvent & PlayerBanWaveEvent

## [0.4.0-rc.9] - 2025-01-19

### Fixed

- Fix item related punishment

## [0.4.0-rc.8] - 2025-01-18

### Fixed

- Fix enchancement check of leggings

## [0.4.0-rc.7] - 2025-01-16

### Fixed

- Fix enchancement check of some items

## [0.4.0-rc.6] - 2025-01-13

### Fixed

- Fix enchancement check of enchaned book

## [0.4.0-rc.5] - 2025-01-12

### Changed

- Support LeviLamina 1.0.0-rc.3

## [0.4.0-rc.4] - 2025-01-10

### Fixed

- Fix antixray chunk block entity
- Fix IllegallyTradeRestrictions [#24]

## [0.4.0-rc.3] - 2025-01-09

### Changed

- Remove illegalMovementCheck->triggerReplayDistance

## [0.4.0-rc.2] - 2025-01-09

### Fixed

- Fix CheckItemNbt [#23]
- Fix AntiXray block update

## [0.4.0-rc.1] - 2025-01-09

### Changed

- Support LeviLamina 1.0.0-rc.2

## [0.3.7] - 2024-08-27

### Added

- Add some measure to improve high packet loss player's experience

### Changed

- Adjust some default configuration

### Fixed

- Fix elytra landing position [#12]

## [0.3.6] - 2024-07-18

### Added

- Add container crash fix
- Add crafter crash fix

## [0.3.5] - 2024-07-14

### Added

- Add configuration reloading

## [0.3.4] - 2024-07-10

### Changed

- Adjust default IllegalMovementCheck's configuration

## [0.3.3] - 2024-07-03

### Changed

- Clean some code

## [0.3.2] - 2024-07-03

### Changed

- Refactoring EmptyPacketFix

### Fixed

- Fix AntiInvalidNbtItem

## [0.3.1] - 2024-06-20

### Added

- Add EmptyPacketFix

## [0.3.0] - 2024-06-19

### Added

- Adapt to LeviLamina 0.13.x

### Changed

- Remove decorated pot loot table fix

## [0.2.7] - 2024-05-26

### Added

- Allow user specified solid blocks

### Fixed

- Handle exception in checkItemNbt

## [0.2.6] - 2024-05-24

### Fixed

- Fix block palette serialization

## [0.2.5] - 2024-05-23

### Changed

- AntiXray: send block update packet manually

### Fixed

- Fix AntiLoginFlood

## [0.2.4] - 2024-05-18

### Fixed

- Fix a problem of AntiXray

## [0.2.3] - 2024-05-07

### Fixed

- Fix AntiXray proxy chunk sync

## [0.2.2] - 2024-05-03

### Fixed

- Try fix an AntiXray's bug

## [0.2.1] - 2024-05-02

### Fixed

- Fix DecoratedPotLootTableFix [#9]

## [0.2.0] - 2024-04-28

### Changed

- Adapt to LeviLamina 0.12.x

## [0.1.5] - 2024-04-26

### Changed

- Revert "Let AntiXRay send block update directly"

## [0.1.4] - 2024-04-22

### Changed

- Let AntiXRay send block update directly
- Use SystemTimeScheduler

## [0.1.3] - 2024-04-18

### Fixed

- Fix event logic
- Fix errorneous judgement of BadPacket
- Fix a logic problem in punish

## [0.1.2] - 2024-04-18

### Added

- Add AntiBadPacket
- Add DecoratedPotLootTableFix
- Add PlayerCheatEvent
- Add PlayerBanWaveEvent
- Add enableBanWave configuration

### Fixed

- Fix AntiXRay hidden block behavior
- Fix AntiXRay solid map
- Fix IllegalBreakingCheck
- Ignore non-standard layer block update

## [0.1.1] - 2024-04-17

### Added

- Add disableSelector config
- Add GatewayCopyFix

### Changed

- Remove ContainerMoveCheck
- Rewrite IllegalMovementCheck

[#9]: https://github.com/LiteLDev/LeviAntiCheat/issues/9
[#12]: https://github.com/LiteLDev/LeviAntiCheat/issues/12
[#23]: https://github.com/LiteLDev/LeviAntiCheat/issues/23
[#24]: https://github.com/LiteLDev/LeviAntiCheat/issues/24
[#25]: https://github.com/LiteLDev/LeviAntiCheat/issues/25

[0.4.5]: https://github.com/LiteLDev/LeviAntiCheat/compare/v0.4.4...v0.4.5
[0.4.4]: https://github.com/LiteLDev/LeviAntiCheat/compare/v0.4.3...v0.4.4
[0.4.3]: https://github.com/LiteLDev/LeviAntiCheat/compare/v0.4.2...v0.4.3
[0.4.2]: https://github.com/LiteLDev/LeviAntiCheat/compare/v0.4.1...v0.4.2
[0.4.1]: https://github.com/LiteLDev/LeviAntiCheat/compare/v0.4.0...v0.4.1
[0.4.0]: https://github.com/LiteLDev/LeviAntiCheat/compare/v0.4.0-rc.11...v0.4.0
[0.4.0-rc.11]: https://github.com/LiteLDev/LeviAntiCheat/compare/v0.4.0-rc.10...v0.4.0-rc.11
[0.4.0-rc.10]: https://github.com/LiteLDev/LeviAntiCheat/compare/v0.4.0-rc.9...v0.4.0-rc.10
[0.4.0-rc.9]: https://github.com/LiteLDev/LeviAntiCheat/compare/v0.4.0-rc.8...v0.4.0-rc.9
[0.4.0-rc.8]: https://github.com/LiteLDev/LeviAntiCheat/compare/v0.4.0-rc.7...v0.4.0-rc.8
[0.4.0-rc.7]: https://github.com/LiteLDev/LeviAntiCheat/compare/v0.4.0-rc.6...v0.4.0-rc.7
[0.4.0-rc.6]: https://github.com/LiteLDev/LeviAntiCheat/compare/v0.4.0-rc.5...v0.4.0-rc.6
[0.4.0-rc.5]: https://github.com/LiteLDev/LeviAntiCheat/compare/v0.4.0-rc.4...v0.4.0-rc.5
[0.4.0-rc.4]: https://github.com/LiteLDev/LeviAntiCheat/compare/v0.4.0-rc.3...v0.4.0-rc.4
[0.4.0-rc.3]: https://github.com/LiteLDev/LeviAntiCheat/compare/v0.4.0-rc.2...v0.4.0-rc.3
[0.4.0-rc.2]: https://github.com/LiteLDev/LeviAntiCheat/compare/v0.4.0-rc.1...v0.4.0-rc.2
[0.4.0-rc.1]: https://github.com/LiteLDev/LeviAntiCheat/compare/v0.3.7...v0.4.0-rc.1
[0.3.7]: https://github.com/LiteLDev/LeviAntiCheat/compare/v0.3.6...v0.3.7
[0.3.6]: https://github.com/LiteLDev/LeviAntiCheat/compare/v0.3.5...v0.3.6
[0.3.5]: https://github.com/LiteLDev/LeviAntiCheat/compare/v0.3.4...v0.3.5
[0.3.4]: https://github.com/LiteLDev/LeviAntiCheat/compare/v0.3.3...v0.3.4
[0.3.3]: https://github.com/LiteLDev/LeviAntiCheat/compare/v0.3.2...v0.3.3
[0.3.2]: https://github.com/LiteLDev/LeviAntiCheat/compare/v0.3.1...v0.3.2
[0.3.1]: https://github.com/LiteLDev/LeviAntiCheat/compare/v0.3.0...v0.3.1
[0.3.0]: https://github.com/LiteLDev/LeviAntiCheat/compare/v0.2.7...v0.3.0
[0.2.7]: https://github.com/LiteLDev/LeviAntiCheat/compare/v0.2.6...v0.2.7
[0.2.6]: https://github.com/LiteLDev/LeviAntiCheat/compare/v0.2.5...v0.2.6
[0.2.5]: https://github.com/LiteLDev/LeviAntiCheat/compare/v0.2.4...v0.2.5
[0.2.4]: https://github.com/LiteLDev/LeviAntiCheat/compare/v0.2.3...v0.2.4
[0.2.3]: https://github.com/LiteLDev/LeviAntiCheat/compare/v0.2.2...v0.2.3
[0.2.2]: https://github.com/LiteLDev/LeviAntiCheat/compare/v0.2.1...v0.2.2
[0.2.1]: https://github.com/LiteLDev/LeviAntiCheat/compare/v0.2.0...v0.2.1
[0.2.0]: https://github.com/LiteLDev/LeviAntiCheat/compare/v0.1.5...v0.2.0
[0.1.5]: https://github.com/LiteLDev/LeviAntiCheat/compare/v0.1.4...v0.1.5
[0.1.4]: https://github.com/LiteLDev/LeviAntiCheat/compare/v0.1.3...v0.1.4
[0.1.3]: https://github.com/LiteLDev/LeviAntiCheat/compare/v0.1.2...v0.1.3
[0.1.2]: https://github.com/LiteLDev/LeviAntiCheat/compare/v0.1.1...v0.1.2
[0.1.1]: https://github.com/LiteLDev/LeviAntiCheat/releases/tag/v0.1.1
