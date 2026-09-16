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
108628	./net
38848	./services
792480	./content
17916	./gpu
291332	./tools
65848	./buildtools
4400	./sandbox
135400	./media
5172	./agents
76056	./docs
104412	./base
1496	./skia
```

## changed list after rework

```
1564628	./.git
5692	./titanium
2532824	./chrome
265644	./v8
81956	./chromeos
503148	./build
26039324	./third_party
3621796	./out
238216	./testing
3294032	./android_webview
494892	./components
```
