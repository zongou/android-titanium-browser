## untouched list

```
./.rustfmt.toml
./.git
./PRESUBMIT_test.py
./storage
./services
./clusterfuzz-data
./codelabs
./.claude
./sandbox
./crypto
./.geminiignore
./fuchsia_web
./styleguide
./DIR_METADATA
./printing
./.gitmodules
./gin
./OWNERS
./chromecast
./.clangd
./cc
./ios_internal
./ATL_OWNERS
./.agents
./CPPLINT.cfg
./dbus
./.gemini
./internal
./headless
./PRESUBMIT.py
./codereview.settings
./url
./.clang-tidy
./.yapfignore
./.git-blame-ignore-revs
./AUTHORS
./WATCHLISTS
./PRESUBMIT_test_mocks.py
./.cursorignore
./ipc
./.vpython3
./signing_keys
./SECURITY_OWNERS
./CODE_OF_CONDUCT.md
./BUILD.gn
./BRANCH_FEATURE_OWNERS
./package.json
./.gn
./mojo
./DEPS
./.gitattributes
./.gitignore
./extensions
./BRANCH_OWNERS
./remoting
./LICENSE.chromium_os
./pdf
./.gitallowed
./google_apis
./CRYPTO_OWNERS
./rlz
./README.md
./.mailmap
./webkit
./device
./infra
./apps
./sql
./clank
./.github
./LICENSE
./.clang-format
./build_overrides
```

## file change process

| file              | cloned  | vanadium_patched | gclient_synced | gclient_hooked | deps_installed | titanium_patched | gn_gened |
| ----------------- | ------- | ---------------- | -------------- | -------------- | -------------- | ---------------- | -------- |
| ./.git            | 1484936 | 1594100          | 1564560        |                |                |                  |          |
| ./net             | 79496   |                  | 108628         |                |                |                  |          |
| ./services        | 38844   | 38848            |                |                |                |                  |          |
| ./titanium        |         | 2024             |                | 5656           |                | 5692             |          |
| ./tools           | 130436  |                  | 291332         |                |                |                  |          |
| ./buildtools      | 668     |                  | 65844          | 65848          |                |                  |          |
| ./chrome          | 1079528 | 1080404          | 1592304        | 2532776        |                | 2532816          |          |
| ./sandbox         | 4392    | 4400             |                |                |                |                  |          |
| ./v8              | 4       |                  | 246068         | 265664         |                |                  |          |
| ./chromeos        | 81944   |                  |                | 81952          |                |                  |          |
| ./media           | 135084  |                  | 135400         |                |                |                  |          |
| ./build           | 13424   | 13284            | 503116         | 503132         |                |                  |          |
| ./agents          | 4172    |                  | 5172           |                |                |                  |          |
| ./third_party     | 2646416 | 2647028          | 25089672       | 26039296       |                |                  |          |
| ./out             |         |                  |                |                |                |                  | 3615016  |
| ./content         | 169788  | 169792           | 792480         |                |                |                  |          |
| ./docs            | 41472   |                  | 76056          |                |                |                  |          |
| ./base            | 39424   | 39432            | 104408         |                |                | 104412           |          |
| ./skia            | 1492    |                  |                | 1496           |                |                  |          |
| ./testing         | 8968    |                  | 237416         | 238220         |                |                  |          |
| ./android_webview | 17616   | 17620            | 3294024        |                |                |                  |          |
| ./components      | 481796  | 481908           | 494880         |                |                |                  |          |
| ./gpu             | 17904   |                  |                | 17916          |                |                  |          |

## patched submodule log

- v8  
  2eacd187 (HEAD) drumbrake: disable support for 32-bit binary compilation
- third_party/search_engines_data/resource  
  f7338b7 (HEAD) Add DuckDuckGo on all regional list of search engines  
  2484f191c566ef92ff78169e31a6528692df4076dd51b19fd05d3fddd881608d  -

## unchanged list after rework

```
./net
./services
./content
./gpu
./tools
./buildtools
./sandbox
./media
./agents
./docs
./base
./skia
```

## changed list after rework

```
./.git
./titanium
./chrome
./v8
./chromeos
./build
./third_party
./out
./testing
./android_webview
./components
```
