<div align="center">

# KFlow Assets

**Static asset pack, served from a CDN.**

[![Deploy](https://github.com/almadar-io/almadar-kflow-assets/actions/workflows/deploy.yml/badge.svg)](https://github.com/almadar-io/almadar-kflow-assets/actions/workflows/deploy.yml)

</div>

Static assets for the KFlow knowledge platform: story illustrations, audio and media files, plus shared board packs under `shared/`. The files are served from https://almadar-kflow-assets.web.app, deployed to Firebase Hosting by CI.

## Where this fits

KFlow Assets is the asset pack for the KFlow product, so [kflow-academy](https://github.com/almadar-io/almadar-kflow-academy) (`apps/kflow`) is highlighted.

```mermaid
flowchart TB
  subgraph kernel["Kernel and substrate"]
    core["orbital-core<br/>IR · evaluator · kernel"]
    canvas["orbital-canvas<br/>2D/3D render primitives"]
  end
  subgraph lang["Language"]
    lolo["orbital-lolo<br/>.lolo → .orb"]
    compiler["orbital-compiler<br/>validate · codegen"]
  end
  subgraph hosts["Shells and hosts"]
    ts["orbital-shell-typescript<br/>web · node · @almadar/core"]
    rs["orbital-shell-rust<br/>desktop · tui"]
    py["orbital-shell-python"]
    ios["orbital-shell-ios"]
    android["orbital-shell-android"]
    os["orbital-shell-os"]
    wasm["orbital-wasm<br/>browser kernel"]
    ffi["orbital-ffi<br/>C ABI for mobile"]
    router["orbital-router"]
  end
  cli["orbital-cli<br/>the orb binary"]
  ws["orbital-rust<br/>workspace · cross-crate tests"]
  dist["orb<br/>npm · releases"]
  subgraph pkgs["Language packages"]
    std["almadar-std<br/>@almadar/std substrate"]
    beh["behaviors<br/>themed organisms"]
    langs["lolo-ar · lolo-sl<br/>language packs"]
  end
  subgraph apps["Apps and sites"]
    builder["builder (studio)"]
    kflow["kflow-academy"]
    nata["nata"]
    rawi["rawi"]
    site["almadar (websites)"]
  end
  core --> lolo & compiler & ts & rs & py & ios & android & os & wasm & ffi & router
  canvas --> ts & rs & ffi
  lolo --> compiler
  compiler --> cli
  ts & rs & py & ios & android & os --> cli
  cli --> dist
  ws -.pins.-> core & lolo & compiler & cli
  dist --> std
  std --> beh
  std --> langs
  beh --> builder & kflow & nata & rawi & site
  click core "https://github.com/almadar-io/orbital-core"
  click canvas "https://github.com/almadar-io/orbital-canvas"
  click lolo "https://github.com/almadar-io/orbital-lolo"
  click compiler "https://github.com/almadar-io/orbital-compiler"
  click ts "https://github.com/almadar-io/orbital-shell-typescript"
  click rs "https://github.com/almadar-io/orbital-shell-rust"
  click py "https://github.com/almadar-io/orbital-shell-python"
  click ios "https://github.com/almadar-io/orbital-shell-ios"
  click android "https://github.com/almadar-io/orbital-shell-android"
  click os "https://github.com/almadar-io/orbital-shell-os"
  click wasm "https://github.com/almadar-io/orbital-wasm"
  click ffi "https://github.com/almadar-io/orbital-ffi"
  click router "https://github.com/almadar-io/orbital-router"
  click cli "https://github.com/almadar-io/orbital-cli"
  click ws "https://github.com/almadar-io/orbital-rust"
  click dist "https://github.com/almadar-io/orb"
  click std "https://github.com/almadar-io/almadar-std"
  click beh "https://github.com/almadar-io/behaviors"
  click langs "https://github.com/almadar-io/lolo-ar"
  click builder "https://github.com/itechdom/almadar-studio"
  click kflow "https://github.com/almadar-io/almadar-kflow-academy"
  click nata "https://github.com/almadar-io/almadar-nata"
  click rawi "https://github.com/almadar-io/almadar-rawi"
  click site "https://github.com/almadar-io/almadar"
  classDef here fill:#2563eb,color:#fff,stroke:#1e40af,stroke-width:3px
  
  class kflow here
```

| Upstream (this repo depends on) | Downstream (depends on this repo) |
|---|---|
| [none](https://github.com/almadar-io/almadar-kflow-assets): a data-only repo | [kflow-academy](https://github.com/almadar-io/almadar-kflow-academy): the KFlow app |

## Quick start

```bash
git clone git@github.com:almadar-io/almadar-kflow-assets.git
cd almadar-kflow-assets
git lfs pull        # large files stay pointer stubs without this
```

Images, audio, video and models are tracked with Git LFS. The CDN root is the repo root: a file at `shared/<board>/<file>` is served at `https://almadar-kflow-assets.web.app/shared/<board>/<file>`.

## What's inside

```
stories/                                      # story illustration assets
shared/                                       # asset packs per UI board (arena, battle, boardgame, ...)
brand/ characters.json manifest.json asset-workflow.json
firebase.json                                 # Hosting target kflow-assets, cache and CORS headers
```

## Development

There is no build and no test suite; the repo is data. Keep the manifests consistent with the files present. `deploy.yml` runs on push to `main` when an image, audio, video, model, PDF, `manifest.json` or `firebase.json` file changes (and on manual dispatch): it pulls the LFS objects, checks that they are real files, and deploys Hosting target `kflow-assets` of project `kflow-b3a39`. Open gaps are in `Almadar_Gaps.md`. Work on `main` only. Manual deploy: `firebase deploy --only hosting:kflow-assets`.

## Docs

- [Orb documentation](https://orb.almadar.io/docs): the language, the `orb` CLI and how the pieces fit

## License
No license file in this repo.
