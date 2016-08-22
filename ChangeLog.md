# Changelog
This changelog is in progress. It can be manually updated via the wiki, but is also updated automatically via select commit messages and new releases. The two comment lines with git hashes (`<!---a1234--->`) must not be changed or removed.

<!---c4f06e44d56e12e5082c7915a11a56cb44e2e32f--->

<!---87914431192b88c1233295ff70a1d5042e610640--->

## 2.3.4 (2016-08-21)
[all commits](https://github.com/Flexget/Flexget/compare/2.3.3...2.3.4)
### Fixed
- search plugins: no longer crashes on single digit sizes eg. "1 GiB", fixes [#1359](https://github.com/Flexget/Flexget/issues/1359)
- irc: cli `status all` now only prints once

### Added
- re-added rutracker plugin


## 2.3.3 (2016-08-20)
[all commits](https://github.com/Flexget/Flexget/compare/2.3.2...2.3.3)
### Added
- irc: added CLI commands for restarting, stopping and checking irc connections


## 2.3.2 (2016-08-19)
[all commits](https://github.com/Flexget/Flexget/compare/2.3.1...2.3.2)
### Fixed
- irc: putting ~ (tilde) in tracker config path no longer fails to find it on disk
- irc: specifying tracker file by name only will no longer fail to find it on disk


## 2.3.1 (2016-08-18)
[all commits](https://github.com/Flexget/Flexget/compare/2.3.0...2.3.1)
### Fixed
- series: Fix crash when using guessit parser on shows with 'Part X' identifiers. fix [#1326](https://github.com/Flexget/Flexget/issues/1326)
- aria2 won't crash on jinja2 render errors
- Make aria2 respect --test mode again.
- aria2 - Fix aria2 plugin on python 3.
- piratebay entry size is now parsed correctly
- api_bluray: bluray lookup and estimator no longer crash when info not found, fixes [#1352](https://github.com/Flexget/Flexget/issues/1352) [#1353](https://github.com/Flexget/Flexget/issues/1353)
- [WebUI] Locked all bower deps to patch level. fixes [#1350](https://github.com/Flexget/Flexget/issues/1350)


## 2.3.0 (2016-08-17)
[all commits](https://github.com/Flexget/Flexget/compare/2.2.22...2.3.0)
### Fixed
- fixed square brackets messing up move's along, fixes [#1348](https://github.com/Flexget/Flexget/issues/1348)
- IMDB List - Added more supported types. Fixes [#1343](https://github.com/Flexget/Flexget/issues/1343)

### Changed
- webrip is now considered better than screeners
- Many CLI commands now have nice formatted table output
- CLI command `flexget trakt show` has been renamed to `flexget trakt list`
- discover `release_estimations` now defaults to `strict` meaning anything with no release date or one that lies in the future will not be included in the search
- discover will now keep searching for new episodes until it fails to find any (maximum 100 runs). Can be set to the old behaviour with `max_reruns` plugin.
- [Aria2](/Plugins/aria2) is drastically simplified and many features are removed.

### Removed
- Removed `movie_queue` and all related plugins.
- Removed `imdb_required` plugin, switch to `imdb_lookup` and `require_field`
- Removed `subtitle_queue` plugin
- Removed `rutracker`  plugin
- Removed `torrentz` plugin
- Removed `newzleech` plugin
- Removed `publichd` plugin
- Removed `bt-chat` plugin
- Removed `btjunkie` plugin
- Removed `isohunt` plugin
- Removed `redskunk` plugin
- Removed `stmusic` plugin

### Added
- added blu-ray.com movie estimator (takes priority over the old one)
- blu-ray.com lookup (`bluray_lookup`)


## 2.2.22 (2016-08-17)
[all commits](https://github.com/Flexget/Flexget/compare/2.2.21...2.2.22)
### Fixed
- html plugin will now properly dump the contents if configured to
- form - Solved TypeError Issue. Fixes [#1344](https://github.com/Flexget/Flexget/issues/1344)


## 2.2.21 (2016-08-16)
[all commits](https://github.com/Flexget/Flexget/compare/2.2.20...2.2.21)
### Fixed
- IMDB list - Added `documentary` type to be parsed as movie. Fixes [#1343](https://github.com/Flexget/Flexget/issues/1343)
- Fuzer - Fixed updated site layout


## 2.2.20 (2016-08-15)
[all commits](https://github.com/Flexget/Flexget/compare/2.2.19...2.2.20)

## 2.2.19 (2016-08-14)
[all commits](https://github.com/Flexget/Flexget/compare/2.2.18...2.2.19)
### Changed
- Allow use of `now` in email plugin templates. fix [#1335](https://github.com/Flexget/Flexget/issues/1335)


## 2.2.18 (2016-08-14)
[all commits](https://github.com/Flexget/Flexget/compare/2.2.17...2.2.18)
### Fixed
- imdb list - Correction IMDb login fixes [#1321](https://github.com/Flexget/Flexget/issues/1321)


## 2.2.17 (2016-08-12)
[all commits](https://github.com/Flexget/Flexget/compare/2.2.16...2.2.17)
### Fixed
- irc: Fixed unicode errors when reading tracker file
- irc: Fixed KeyError when extracting tags from announcement

### Changed
- irc: tracker_file option is no longer case sensitive nor does it require .tracker extension


## 2.2.16 (2016-08-11)
[all commits](https://github.com/Flexget/Flexget/compare/2.2.15...2.2.16)
### Added
- Plex - Added two new fields


## 2.2.15 (2016-08-10)
[all commits](https://github.com/Flexget/Flexget/compare/2.2.14...2.2.15)
### Fixed
- Pushbullet: Fixed api key being invalid in Py3, fixes [#1320](https://github.com/Flexget/Flexget/issues/1320)


## 2.2.14 (2016-08-09)
[all commits](https://github.com/Flexget/Flexget/compare/2.2.13...2.2.14)
### Fixed
- tvmaze and tmdb caches are no longer cleared on each run


## 2.2.13 (2016-08-09)
[all commits](https://github.com/Flexget/Flexget/compare/2.2.12...2.2.13)
### Fixed
- Fixed crash in trakt plugins with latest version of requests library.


## 2.2.12 (2016-08-08)
[all commits](https://github.com/Flexget/Flexget/compare/2.2.11...2.2.12)

## 2.2.11 (2016-08-07)
[all commits](https://github.com/Flexget/Flexget/compare/2.2.10...2.2.11)
### Fixed
- move - 'files' and 'subdirs' no longer crash on single strings
- html - fixed regular expr used to create title from url, really fixes [#1250](https://github.com/Flexget/Flexget/issues/1250)

### Changed
- Subliminal plugin now finds embedded subtitles (again). Also fixed single mode when found language is undefined.

### Added
- Prowl - Allow the sending of the prowl url parameter


## 2.2.10 (2016-08-07)
[all commits](https://github.com/Flexget/Flexget/compare/2.2.9...2.2.10)
### Added
- Plex - Populate series info for Plex episodes


## 2.2.9 (2016-08-05)
[all commits](https://github.com/Flexget/Flexget/compare/2.2.8...2.2.9)
### Fixed
- Html plugin can create titles from magnet links again. fixes [#1250](https://github.com/Flexget/Flexget/issues/1250)


## 2.2.8 (2016-08-04)
[all commits](https://github.com/Flexget/Flexget/compare/2.2.7...2.2.8)

## 2.2.7 (2016-08-03)
[all commits](https://github.com/Flexget/Flexget/compare/2.2.6...2.2.7)

## 2.2.6 (2016-08-03)
[all commits](https://github.com/Flexget/Flexget/compare/1501a7d622a3fff4dd9588cda8e15dfe770791b6...0d110294637c5edd42dbf63179b3595dfa8e43c2)

## 2.2.5 (2016-08-02)
[all commits](https://github.com/Flexget/Flexget/compare/c79e6c077a76bf810ccbdb2715c92cfa86064248...1501a7d622a3fff4dd9588cda8e15dfe770791b6)
### Fixed
- Requrie a version of Beautifulsoup4 that can handle different html5lib versions. fix [#1309](https://github.com/Flexget/Flexget/issues/1309)


## 2.2.4 (2016-08-01)
[all commits](https://github.com/Flexget/Flexget/compare/7926bcc5da24cbbe9e689c19a940aa3862aca7be...c79e6c077a76bf810ccbdb2715c92cfa86064248)
### Fixed
- 'local' is now strictly a boolean


## 2.2.3 (2016-07-31)
[all commits](https://github.com/Flexget/Flexget/compare/426fe0bf6611fc4fde00db0687ec33708943808c...7926bcc5da24cbbe9e689c19a940aa3862aca7be)
### Fixed
- tvmaze_api - Removed searching from cache via airdate. Fixes [#1305](https://github.com/Flexget/Flexget/issues/1305)


## 2.2.2 (2016-07-29)
[all commits](https://github.com/Flexget/Flexget/compare/19f63cfabcf1b7d877661841539dac642784792e...426fe0bf6611fc4fde00db0687ec33708943808c)

## 2.2.1 (2016-07-28)
[all commits](https://github.com/Flexget/Flexget/compare/986aa70f9bc80209adc796ec14a3a0730baa6ef0...19f63cfabcf1b7d877661841539dac642784792e)

## 2.2.0 (2016-07-27)
[all commits](https://github.com/Flexget/Flexget/compare/ef190de036680eee0826abe4c1604e37676e3f86...986aa70f9bc80209adc796ec14a3a0730baa6ef0)
### Fixed
- require_field - Improve check logic.
- require_field - Do not implicitly convert to bool.

### Changed
- move/copy/delete 'along' now supports subdirs


## 2.1.25 (2016-07-26)
[all commits](https://github.com/Flexget/Flexget/compare/9342a97dd33817bde8036fa033bcf92f5affbaa7...ef190de036680eee0826abe4c1604e37676e3f86)
### Fixed
- [WebUI] Series episodes block incorrectly cutting of series row
- list match - Tighter schema
- **plugins API** - Makes args case insensitive


## 2.1.24 (2016-07-25)
[all commits](https://github.com/Flexget/Flexget/compare/ff7845498973ad60e44ea1ced9f1c406d050d4d8...9342a97dd33817bde8036fa033bcf92f5affbaa7)
### Fixed
- **fuzer** - Did not return results correctly


## 2.1.23 (2016-07-24)
[all commits](https://github.com/Flexget/Flexget/compare/a95e40937a4d5a5efce0302fb04d671d27cb832f...ff7845498973ad60e44ea1ced9f1c406d050d4d8)
### Fixed
- Make tail plugin work consistenly with unicode on py2/3. fix [#1269](https://github.com/Flexget/Flexget/issues/1269)
- telegram - Changed plugin to be an output plugin and not an exit plugin
- database API - Fixed return object to be a list

### Changed
- Tail plugin defaults to utf8 instead of ascii encoding


## 2.1.22 (2016-07-23)
[all commits](https://github.com/Flexget/Flexget/compare/ae8ef4e20e36b90ca2896bdc123ebb09f89f0a88...a95e40937a4d5a5efce0302fb04d671d27cb832f)

## 2.1.21 (2016-07-23)
[all commits](https://github.com/Flexget/Flexget/compare/69f3550e7fd600727150e32f63f004d7c590b458...ae8ef4e20e36b90ca2896bdc123ebb09f89f0a88)
### Fixed
- changed pushbullet error logging, fixes [#1225](https://github.com/Flexget/Flexget/issues/1225)
- irc will now properly try to reconnect again
- IMDB list - Correctly set type for different IMDB entities. Fixes [#1270](https://github.com/Flexget/Flexget/issues/1270)
- clean_source now uses old location, fixes  [#1284](https://github.com/Flexget/Flexget/issues/1284)
- Stricter episode matching, finally fixes [#1111](https://github.com/Flexget/Flexget/issues/1111)
- thetvdb_favorites deprecation message no longer shows for thetvdb_list
- fuzer - Changed logic to use the new search API

### Changed
- added web quality, closes [#1218](https://github.com/Flexget/Flexget/issues/1218)
- fuzer -Refactor and added support for search via imdb_id


## 2.1.20 (2016-07-22)
[all commits](https://github.com/Flexget/Flexget/compare/c6cd875e4f2a686266ab3f254cb55ab12801d3ba...69f3550e7fd600727150e32f63f004d7c590b458)
### Fixed
- changed pushbullet error logging, fixes [#1225](https://github.com/Flexget/Flexget/issues/1225)
- irc will now properly try to reconnect again
- manual plugin - Manual plugin never aborted any task. Fixes [#1291](https://github.com/Flexget/Flexget/issues/1291)

### Changed
- added web quality, closes [#1218](https://github.com/Flexget/Flexget/issues/1218)


## 2.1.19 (2016-07-21)
[all commits](https://github.com/Flexget/Flexget/compare/0c951c0d5630c2450151d371265599c5e89990c7...c6cd875e4f2a686266ab3f254cb55ab12801d3ba)

## 2.1.18 (2016-07-20)
[all commits](https://github.com/Flexget/Flexget/compare/da6f88c37348b48879ff84679cb93e72185a0d0c...0c951c0d5630c2450151d371265599c5e89990c7)

## 2.1.17 (2016-07-19)
[all commits](https://github.com/Flexget/Flexget/compare/d0cb205a7e1cb370bb897a73c4855231e8d609c3...da6f88c37348b48879ff84679cb93e72185a0d0c)
### Fixed
- IMDB list - Correctly set type for different IMDB entities. Fixes [#1270](https://github.com/Flexget/Flexget/issues/1270)
- clean_source now uses old location, fixes  [#1284](https://github.com/Flexget/Flexget/issues/1284)


## 2.1.16 (2016-07-18)
[all commits](https://github.com/Flexget/Flexget/compare/79b16409667d233f4abb9a65496602759156031e...d0cb205a7e1cb370bb897a73c4855231e8d609c3)
### Changed
- fuzer -Refactor and added support for search via imdb_id

### Fixed
- Stricter episode matching, finally fixes [#1111](https://github.com/Flexget/Flexget/issues/1111)


## 2.1.15 (2016-07-17)
[all commits](https://github.com/Flexget/Flexget/compare/481ddcd11c9707656b013191cb0eb1c39c90d43b...79b16409667d233f4abb9a65496602759156031e)
### Fixed
- thetvdb_favorites deprecation message no longer shows for thetvdb_list
- fuzer - Changed logic to use the new search API
- fuzer - Fixed incorrect search pattern

### Changed
- Allow manipulate to run in modify phase
- Allow setting filename with config in download plugin


## 2.1.14 (2016-07-17)
[all commits](https://github.com/Flexget/Flexget/compare/da203f0bf763280d8555e06270dd70ef965034ef...481ddcd11c9707656b013191cb0eb1c39c90d43b)
### Changed
- only join chan on invite if it's in the list


## 2.1.13 (2016-07-15)
[all commits](https://github.com/Flexget/Flexget/compare/2bbda3456e5e8aff3cefa2c4f988017ca24a52cd...da203f0bf763280d8555e06270dd70ef965034ef)
### Fixed
- Pin html5lib version to prevent bs4 bug.


## 2.1.12 (2016-07-14)
[all commits](https://github.com/Flexget/Flexget/compare/409b4b193182f4d0330d055e8399e69ea6868af8...2bbda3456e5e8aff3cefa2c4f988017ca24a52cd)
### Changed
- no more log "spam", rip decorator


## 2.1.11 (2016-07-13)
[all commits](https://github.com/Flexget/Flexget/compare/9550514bc323c92dfe171e60588e80281223f77d...409b4b193182f4d0330d055e8399e69ea6868af8)
### Fixed
- irc plugin will not try to hash an empty config, fixes [#1274](https://github.com/Flexget/Flexget/issues/1274)
- operation did not complete read fixed


## 2.1.10 (2016-07-13)
[all commits](https://github.com/Flexget/Flexget/compare/aa7f859d1dc20bee818250f38059fe63d24de73f...9550514bc323c92dfe171e60588e80281223f77d)

## 2.1.9 (2016-07-11)
[all commits](https://github.com/Flexget/Flexget/compare/908866d0271d3d3a62007875c67746b1a882a415...aa7f859d1dc20bee818250f38059fe63d24de73f)
### Fixed
- Fuzer Encode password before hashing

### Changed
- download and move now set 'location' field


## 2.1.8 (2016-07-11)
[all commits](https://github.com/Flexget/Flexget/compare/47227877cb277bdcd2bd0f53a88f07b5116faa78...908866d0271d3d3a62007875c67746b1a882a415)

## 2.1.7 (2016-07-07)
[all commits](https://github.com/Flexget/Flexget/compare/9f55caa5fb82090fa362175cfb09e4fd89444e9a...47227877cb277bdcd2bd0f53a88f07b5116faa78)
### Added
- qbittorent - Added ability to not fail html content links

### Fixed
- tvdb - TVDB lookup did not correctly lookup specials.
- tail - Open file as binary. Fixes [#1269](https://github.com/Flexget/Flexget/issues/1269)


## 2.1.6 (2016-07-04)
[all commits](https://github.com/Flexget/Flexget/compare/0d0c20399132d147c586060b9d67cc37102b949c...9f55caa5fb82090fa362175cfb09e4fd89444e9a)
### Fixed
- movie list - explicitly check for movie year. Fixes [#1266](https://github.com/Flexget/Flexget/issues/1266)


## 2.1.5 (2016-07-04)
[all commits](https://github.com/Flexget/Flexget/compare/73b1bf8c9077de0195b12896e20a94949283056d...0d0c20399132d147c586060b9d67cc37102b949c)
### Fixed
- api - Added missing swagger error schema doc for py3
- execute api - Fixed no_cache attribute not stored as expected
- telegram - Fixed telegram error import. Fixes [#1262](https://github.com/Flexget/Flexget/issues/1262)

### Added
- kat - Added anime category


## 2.1.4 (2016-06-29)
[all commits](https://github.com/Flexget/Flexget/compare/4730666e772c0be37a3035f03a208c8df31ff265...73b1bf8c9077de0195b12896e20a94949283056d)

## 2.1.3 (2016-06-28)
[all commits](https://github.com/Flexget/Flexget/compare/a7c6ff200ccb235621994e498f772b443320a506...4730666e772c0be37a3035f03a208c8df31ff265)
### Fixed
- tl - Catch request errors


## 2.1.2 (2016-06-28)
[all commits](https://github.com/Flexget/Flexget/compare/b96962025006ed2a1c6732f0e384d626d1e808ea...a7c6ff200ccb235621994e498f772b443320a506)
### Changed
- allow_dir is only used when adding to the subtitle list

### Fixed
- raw_config - Made endpoint much more robust


## 2.1.1 (2016-06-24)
[all commits](https://github.com/Flexget/Flexget/compare/c76026cdf6b62a8ba326f65496b80788fd34bb84...b96962025006ed2a1c6732f0e384d626d1e808ea)

## 2.1.0 (2016-06-23)
[all commits](https://github.com/Flexget/Flexget/compare/8650012fc0b8aa04756090a01ed86edb6448a90c...c76026cdf6b62a8ba326f65496b80788fd34bb84)
### Fixed
- raw_config API - Fixed py3 compatibility
- API - Response description cannot be null, default is now `Success`. Fixes [#1182](https://github.com/Flexget/Flexget/issues/1182)


## 2.0.51 (2016-06-22)
[all commits](https://github.com/Flexget/Flexget/compare/1727d5618aac4606d506963e78efdd6ee74f2e94...8650012fc0b8aa04756090a01ed86edb6448a90c)
### Fixed
- fixed bad if-statement regarding trakt_released, fixes [#1236](https://github.com/Flexget/Flexget/issues/1236)


## 2.0.50 (2016-06-22)
[all commits](https://github.com/Flexget/Flexget/compare/4aa58b8fb2dfe28239834b035da973a695d68ed0...1727d5618aac4606d506963e78efdd6ee74f2e94)
### Fixed
- Force empty list instead of None in genres and translations, fixes [#1219](https://github.com/Flexget/Flexget/issues/1219)

### Added
- server/raw_config - Added raw config endpoint


## 2.0.49 (2016-06-20)
[all commits](https://github.com/Flexget/Flexget/compare/a786a62de34487bf771d20111ca342170b966473...4aa58b8fb2dfe28239834b035da973a695d68ed0)
### Fixed
- transmission plugin on python 2 with non-ascii paths fix [#1237](https://github.com/Flexget/Flexget/issues/1237)


## 2.0.48 (2016-06-16)
[all commits](https://github.com/Flexget/Flexget/compare/a06552448280d146842b51d82dadad9004eaa2b5...a786a62de34487bf771d20111ca342170b966473)
### Changed
- trakt lookup - Changed some trakt lookup fields to correctly reflect data
- movie list - Added ability for movie list to parse movie title if no identifiers were present

### Added
- added some requested features to subtitle_list, closes [#1224](https://github.com/Flexget/Flexget/issues/1224)


## 2.0.47 (2016-06-16)
[all commits](https://github.com/Flexget/Flexget/compare/dbc2d97f5268b2170a5b55694d3035304b616258...a06552448280d146842b51d82dadad9004eaa2b5)
### Fixed
- entry list CLI - Made entry list CLI syntax consistent with movie list CLI

### Added
- metainfo_movie - Added metainfo_movie plugin


## 2.0.46 (2016-06-14)
[all commits](https://github.com/Flexget/Flexget/compare/3edeedd2a5e3dc1a6a34415c56afc040c768d2bb...dbc2d97f5268b2170a5b55694d3035304b616258)
### Fixed
- newznab - Correctly search for series name. Fixes [#1217](https://github.com/Flexget/Flexget/issues/1217)
- API - Custom JSON formats and blank payload passed non serializable error messages. Fixes [#1235](https://github.com/Flexget/Flexget/issues/1235)


## 2.0.45 (2016-06-14)
[all commits](https://github.com/Flexget/Flexget/compare/0ffe9ffbc71cedb589569e95b631a8ea6874d731...3edeedd2a5e3dc1a6a34415c56afc040c768d2bb)

## 2.0.44 (2016-06-13)
[all commits](https://github.com/Flexget/Flexget/compare/95461c2a8ebff6d65e5846df9872d1274eb66cac...0ffe9ffbc71cedb589569e95b631a8ea6874d731)
### Added
- movie list - Added `added` attribute to movie entry


## 2.0.43 (2016-06-13)
[all commits](https://github.com/Flexget/Flexget/compare/275a162ef94e227f7dac70425b73a0113b0a3219...95461c2a8ebff6d65e5846df9872d1274eb66cac)
### Fixed
- fix pushbullet crash on python 3 fix [#1225](https://github.com/Flexget/Flexget/issues/1225)
- crash with html input plugin when generating titles from url. fix [#1227](https://github.com/Flexget/Flexget/issues/1227)
- Transmission plugin now works properly on python 3. fix [#1100](https://github.com/Flexget/Flexget/issues/1100)


## 2.0.42 (2016-06-11)
[all commits](https://github.com/Flexget/Flexget/compare/d240ee56641d6aab62d81aad82558c2224473882...275a162ef94e227f7dac70425b73a0113b0a3219)
### Fixed
- return response from get wrapper


## 2.0.41 (2016-06-07)
[all commits](https://github.com/Flexget/Flexget/compare/3452e801f35e61c2530ad8c3fbf69f3bb1e84c31...d240ee56641d6aab62d81aad82558c2224473882)

## 2.0.40 (2016-06-02)
[all commits](https://github.com/Flexget/Flexget/compare/001deaac46bf44198ce27f160e91f664e3e0df64...3452e801f35e61c2530ad8c3fbf69f3bb1e84c31)
### Fixed
- Revert " qualities - Add regex to correctly match webrip quality. Fixes [#1218](https://github.com/Flexget/Flexget/issues/1218)"
- qualities - Add regex to correctly match webrip quality. Fixes [#1218](https://github.com/Flexget/Flexget/issues/1218)


## 2.0.39 (2016-06-01)
[all commits](https://github.com/Flexget/Flexget/compare/6a77ca315dae0c40d384aca5ec7d47ed45a7d97a...001deaac46bf44198ce27f160e91f664e3e0df64)
### Fixed
- imdb list -Forgot sending cookies with list fetch requests
- newnzab - Fixed forcing tvrage ID to be mandatory. Fixes [#1217](https://github.com/Flexget/Flexget/issues/1217)
- API - Change all endpoints to include a trailing slash. Fixes [#1215](https://github.com/Flexget/Flexget/issues/1215)


## 2.0.38 (2016-05-31)
[all commits](https://github.com/Flexget/Flexget/compare/83146096b038ac9fecc5e0d5d9ec1fda2f1e29d7...6a77ca315dae0c40d384aca5ec7d47ed45a7d97a)

## 2.0.37 (2016-05-30)
[all commits](https://github.com/Flexget/Flexget/compare/526de34606ba0f002bd3a0ac3e592f0d04fb7740...83146096b038ac9fecc5e0d5d9ec1fda2f1e29d7)
### Fixed
- - sceper - Wrong string format. Fixes [#1210](https://github.com/Flexget/Flexget/issues/1210)
- flask - Updated calling flask.ext to new method due to flask upgrade to 0.11 to get rid of deprecation warning.
- - imdb_list - Enabled imdb_list to cache credentials per login name ([#1209](https://github.com/Flexget/Flexget/issues/1209)). Fixes [#1109](https://github.com/Flexget/Flexget/issues/1109)


## 2.0.36 (2016-05-30)
[all commits](https://github.com/Flexget/Flexget/compare/062b5a36b9ecdf47eca17e90972430833d7b4020...526de34606ba0f002bd3a0ac3e592f0d04fb7740)
### Fixed
- iptorrents - Fix invalid search string generation, update base_url to use HTTPS


## 2.0.35 (2016-05-28)
[all commits](https://github.com/Flexget/Flexget/compare/4f3e816515d3fe8e21760234f9059013ef077e99...062b5a36b9ecdf47eca17e90972430833d7b4020)

## 2.0.34 (2016-05-26)
[all commits](https://github.com/Flexget/Flexget/compare/9834ccdf821544d23045f57ce6cc717b0a083c94...4f3e816515d3fe8e21760234f9059013ef077e99)

## 2.0.33 (2016-05-25)
[all commits](https://github.com/Flexget/Flexget/compare/62fecfcb83db0f83d430c6c2e80906d232fac3ae...9834ccdf821544d23045f57ce6cc717b0a083c94)
### Fixed
- - movie_list - Added ability to strip_year. Closes [#1128](https://github.com/Flexget/Flexget/issues/1128)


## 2.0.32 (2016-05-25)
[all commits](https://github.com/Flexget/Flexget/compare/c70354070ff5754675f0b1f46b9048310b2f6e77...62fecfcb83db0f83d430c6c2e80906d232fac3ae)
### Fixed
- thetvdb_lookup - api_tvdb did not support date type series lookups. Fixed [#1036](https://github.com/Flexget/Flexget/issues/1036)


## 2.0.31 (2016-05-24)
[all commits](https://github.com/Flexget/Flexget/compare/08e651b880ac7ce3a0b81775c3035ed18bcf39cb...c70354070ff5754675f0b1f46b9048310b2f6e77)

## 2.0.30 (2016-05-22)
[all commits](https://github.com/Flexget/Flexget/compare/2829c33cc6f224595a927f9f665c0ecccb49de27...08e651b880ac7ce3a0b81775c3035ed18bcf39cb)

## 2.0.29 (2016-05-22)
[all commits](https://github.com/Flexget/Flexget/compare/707074dde18cacfb16bec0a3876ce0c38785ca60...2829c33cc6f224595a927f9f665c0ecccb49de27)

## 2.0.28 (2016-05-20)
[all commits](https://github.com/Flexget/Flexget/compare/9beccc2fc78e66e82c298c4ef3fc92890554e689...707074dde18cacfb16bec0a3876ce0c38785ca60)

## 2.0.27 (2016-05-19)
[all commits](https://github.com/Flexget/Flexget/compare/e3220ba202bb9c08ebe3c9e5466d955c6cfef93b...9beccc2fc78e66e82c298c4ef3fc92890554e689)
### Removed
- send_telegram - Removed telegram CLI operations as they were accessing config directly

### Fixed
- - exec - Now function was needlessly added to global jinja2 env. Fixes [#878](https://github.com/Flexget/Flexget/issues/878)


## 2.0.26 (2016-05-18)
[all commits](https://github.com/Flexget/Flexget/compare/a3f1642d5e55df7befd60561c818a27013cd0c5c...e3220ba202bb9c08ebe3c9e5466d955c6cfef93b)
### Fixed
- Fix bad search results from t411 plugin. fix [#1178](https://github.com/Flexget/Flexget/issues/1178)
- execute API - Correctly pass `now` option. Closes [#1132](https://github.com/Flexget/Flexget/issues/1132)


## 2.0.25 (2016-05-17)
[all commits](https://github.com/Flexget/Flexget/compare/911b48dbfe710df447493e7392d819bba023fb98...a3f1642d5e55df7befd60561c818a27013cd0c5c)
### Fixed
- trakt api - Translations lookup was too broad
- trakt lookup - Translations lookup was incorrect, added test
- ftp_list -Fixed param name
- ftp_list - Added logic to avoid unnecessary recursion

### Added
- - trakt lookup API - Added ability to return translations

### Changed
- trakt lookup API - Changed movies endpoint url


## 2.0.24 (2016-05-17)
[all commits](https://github.com/Flexget/Flexget/compare/542e9f9d983c7803545da9f2e8ce8110452f9c5c...911b48dbfe710df447493e7392d819bba023fb98)
### Fixed
- save search results in lowercase, fixes [#1186](https://github.com/Flexget/Flexget/issues/1186)
- simple_persistence upgrade, fixes [#1133](https://github.com/Flexget/Flexget/issues/1133)
- - cron_env - Lower case string comparison. Fixes [#1185](https://github.com/Flexget/Flexget/issues/1185)
- ftp_list - No longer iterating over all dirs, added options for recursion and recursion depth. Closed [#1162](https://github.com/Flexget/Flexget/issues/1162)
- Only send savepath and label to QBittorrent if available, fixes [#1166](https://github.com/Flexget/Flexget/issues/1166)

### Changed
- movie_list CLI - Added movie lookup and set default movie list name to `movies`
- movie_list CLI - Made `list_name` and `movie_title` positional params
- ftp_list - Changed `use_ssl` to just `ssl`
- ftp_list - Removed `regexp` option as filtering should be done on filter phase


## 2.0.23 (2016-05-15)
[all commits](https://github.com/Flexget/Flexget/compare/124ffa67dcee4848086351f33ed26e745ecabf48...542e9f9d983c7803545da9f2e8ce8110452f9c5c)

## 2.0.22 (2016-05-15)
[all commits](https://github.com/Flexget/Flexget/compare/912cfbde0a2fe25804d4a5c2d11be1f22bfb411b...124ffa67dcee4848086351f33ed26e745ecabf48)

## 2.0.21 (2016-05-13)
[all commits](https://github.com/Flexget/Flexget/compare/108fe75531c42e75623e033aa00c2150b04f0a6b...912cfbde0a2fe25804d4a5c2d11be1f22bfb411b)

## 2.0.20 (2016-05-12)
[all commits](https://github.com/Flexget/Flexget/compare/d2c089b7763a8d99afb58822f6d7063c674322b4...108fe75531c42e75623e033aa00c2150b04f0a6b)

## 2.0.19 (2016-05-11)
[all commits](https://github.com/Flexget/Flexget/compare/ac79ec11a0f2dbf9968a21c23f00605d8beb1721...d2c089b7763a8d99afb58822f6d7063c674322b4)
### Fixed
- quality plugin now recognizes 'unknown' quality as a quality.


## 2.0.18 (2016-05-11)
[all commits](https://github.com/Flexget/Flexget/compare/0b195dd77be7feeb2dce071d9787beff1c334c63...ac79ec11a0f2dbf9968a21c23f00605d8beb1721)
### Fixed
- fix crash in torrent_alive fix [#1117](https://github.com/Flexget/Flexget/issues/1117)


## 2.0.17 (2016-05-10)
[all commits](https://github.com/Flexget/Flexget/compare/066dd7fedba43031f3fbce61b534e0cc472149ab...0b195dd77be7feeb2dce071d9787beff1c334c63)
### Changed
- trakt API - Made actors attribute optional


## 2.0.16 (2016-05-09)
[all commits](https://github.com/Flexget/Flexget/compare/99a779e57e00247c3d21ddf737956ae419fd7dc8...066dd7fedba43031f3fbce61b534e0cc472149ab)
### Fixed
- tvmaze_api - Check if series has image attribute. Closes [#1153](https://github.com/Flexget/Flexget/issues/1153)


## 2.0.15 (2016-05-09)
[all commits](https://github.com/Flexget/Flexget/compare/2685c733fdca05032621d8ed49efae2967ae0608...99a779e57e00247c3d21ddf737956ae419fd7dc8)
### Fixed
- only try to use device authorization when called from cli


## 2.0.14 (2016-05-06)
[all commits](https://github.com/Flexget/Flexget/compare/8cb1d9a725eb1d1bdddd499a6061609d1d7e737e...2685c733fdca05032621d8ed49efae2967ae0608)

## 2.0.13 (2016-05-06)
[all commits](https://github.com/Flexget/Flexget/compare/28e712db5aaa8361288ff18557a51c8080df4eb7...8cb1d9a725eb1d1bdddd499a6061609d1d7e737e)

## 2.0.12 (2016-05-05)
[all commits](https://github.com/Flexget/Flexget/compare/6c9901d26b8f59c3535e150f92e4497cabfa56b0...28e712db5aaa8361288ff18557a51c8080df4eb7)
### Fixed
- trakt_lookup API - Fixed API doc for trakt
- trakt_lookup API - Fixed correct date and time object conversions
- movie list - Check for missing movie name before trying to find entry


## 2.0.11 (2016-05-04)
[all commits](https://github.com/Flexget/Flexget/compare/0efcabd42caef081194bc2fe448fb283462806b9...6c9901d26b8f59c3535e150f92e4497cabfa56b0)
### Fixed
- - execute/inject API - Actually pass the options for execution now. Fixed [#1125](https://github.com/Flexget/Flexget/issues/1125), Fixed [#1132](https://github.com/Flexget/Flexget/issues/1132)
- tvmaze API - Remove usage of actors property
- movie list - Fix crash due to incorrect movie name setting and fixed matching via entry IDs

### Changed
- [subliminal] Add option to save to another directory


## 2.0.10 (2016-05-04)
[all commits](https://github.com/Flexget/Flexget/compare/f4de533b15627d2d8a84e6ff2f227ef6889c0115...0efcabd42caef081194bc2fe448fb283462806b9)
### Fixed
- movie_list - titles are now compared in lower case


## 2.0.9 (2016-05-02)
[all commits](https://github.com/Flexget/Flexget/compare/6c356e12758c2121a4f4fb5d9eaeb44fdb9cebbc...f4de533b15627d2d8a84e6ff2f227ef6889c0115)
### Fixed
- Movie List CLI - Added identifier  type validation. Closed [#1116](https://github.com/Flexget/Flexget/issues/1116)
- use native_str_to_text to ensure text fixs [#1097](https://github.com/Flexget/Flexget/issues/1097)


## 2.0.8 (2016-04-29)
[all commits](https://github.com/Flexget/Flexget/compare/94d7e76bbb50e1611e542969f3ed8f0fcbdc6d6d...6c356e12758c2121a4f4fb5d9eaeb44fdb9cebbc)

## 2.0.7 (2016-04-28)
[all commits](https://github.com/Flexget/Flexget/compare/02152ed46ed9dacd6359851e3db54c3b1693403f...94d7e76bbb50e1611e542969f3ed8f0fcbdc6d6d)

## 2.0.6 (2016-04-27)
[all commits](https://github.com/Flexget/Flexget/compare/a06b3d38873db2555143aadeb8931f36586c83af...02152ed46ed9dacd6359851e3db54c3b1693403f)
### Fixed
- Fix crash with sabnzbd plugin on 2.0+ Fix [#1099](https://github.com/Flexget/Flexget/issues/1099)
- Error reporting and fix. Fix [#1099](https://github.com/Flexget/Flexget/issues/1099)


## 2.0.5 (2016-04-26)
[all commits](https://github.com/Flexget/Flexget/compare/f4dba25f09c351f5411b9e28bafac432a1a43fa1...a06b3d38873db2555143aadeb8931f36586c83af)
