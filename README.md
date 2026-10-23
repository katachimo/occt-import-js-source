# occt-import-js 0.0.23 + Open CASCADE Technology 7.6.1 — corresponding source

This repository holds an **unmodified copy** of the source code of the LGPL-licensed library that
[katachimo](https://katachimo.com/) uses to open STEP / IGES files. It is published so that
anyone who receives the library from katachimo can obtain its complete corresponding source, as
required by the GNU Lesser General Public License version 2.1.

katachimo's own code is not part of this repository.

## What is here

| Directory | Upstream | Version |
|---|---|---|
| `occt-import-js-0.0.23/` | [kovacsv/occt-import-js](https://github.com/kovacsv/occt-import-js) | tag `0.0.23` (commit `c2148e54b456b571238d35cac037d304053d64b2`) |
| `occt-import-js-0.0.23/occt/` | [Open CASCADE Technology](https://github.com/Open-Cascade-SAS/OCCT) (git submodule of the above) | commit `d2abb6d844231cb8f29be6894440874a4700e4a5` ("Update version up to 7.6.1") |

The submodule in occt-import-js points to `https://git.dev.opencascade.org/repos/occt.git`, which
could not be reached on 2026-10-10. The same commit was taken from the official GitHub repository
`Open-Cascade-SAS/OCCT` and placed in `occt/` as plain files. Git history (`.git`) is not included.

Nothing has been changed. Build scripts are in `occt-import-js-0.0.23/tools/` and
`occt-import-js-0.0.23/CMakeLists.txt` (Emscripten; see the upstream README).

## Files katachimo distributes

katachimo serves these files from `occt-import-js-0.0.23/dist/` without modification:

| File | SHA-256 |
|---|---|
| `occt-import-js.js` | `8b090be386bc8ffba32222aa19f38742ae8ed35707819beb7f8ab4938a28c97a` |
| `occt-import-js.wasm` | `33391fc9d94ea5c869a6718488bf0a9a464222bac9bdc764dfe1690cef281952` |
| `license.occt.txt` | `e237fa56668030e928551ddd60f05df5fe957f75eab874bbd017e085ed722e7c` |
| `LICENSE.md` (repository root of occt-import-js) | `20c17d8b8c48a600800dfd14f95d5cb9ff47066a9641ddeab48dc54aec96e331` |

They are loaded only when you open a STEP or IGES file, as separate files. You may replace them
with a modified build of your own.

## Licenses

- occt-import-js: GNU LGPL 2.1 — `occt-import-js-0.0.23/LICENSE.md`
- Open CASCADE Technology: GNU LGPL 2.1 with the Open CASCADE exception —
  `occt-import-js-0.0.23/occt/LICENSE_LGPL_21.txt`, `occt-import-js-0.0.23/occt/OCCT_LGPL_EXCEPTION.txt`
- The JavaScript file includes the Emscripten runtime (MIT License).

---

# 日本語

[katachimo](https://katachimo.com/) が STEP / IGES の読込に使っている LGPL のライブラリの、
**未改変のソースの写し**です。LGPL 2.1 に従い、katachimo からこのライブラリを受け取った人が
対応するソースを入手できるように公開しています。katachimo 本体のコードは含みません。

- `occt-import-js-0.0.23/`: occt-import-js のタグ `0.0.23`
- `occt-import-js-0.0.23/occt/`: Open CASCADE Technology のコミット `d2abb6d`(7.6.1)。
  サブモジュールの接続先に 2026-10-10 時点でつながらなかったため、公式の GitHub
  (`Open-Cascade-SAS/OCCT`)から同じコミットを取り、ファイルとして置いています
- 変更は加えていません。katachimo が配信している `dist/` のファイルの SHA-256 は上の表のとおりです
- これらのファイルは STEP / IGES を開いたときだけ別ファイルとして読み込まれ、自分でビルドした
  改変版に差し替えて使うことができます
