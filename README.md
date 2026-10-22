# Switching Heroes 5.60 — Raw APKs, Native Binaries & Asset Bundles

Upstream raw materials for **Switching Heroes** (`com.zilliongames.collectionidle` v5.60, Unity 6000.2.15f1 + IL2CPP + Addressables).

Sister repo with extraction scripts, tooling, and decoded output:
👉 [**`v-reza/switchingheroes-re`**](https://github.com/v-reza/switchingheroes-re)

## Files tracked

Heavy files (>100 MB) are managed via **Git LFS**:

| Path | Size | Description | Tracking |
|---|---:|---|---|
| `Switching+Heroes_5.60_APKPure.xapk` | 280 MB | Upstream source package (sha256: `bc3ee4d63cba0b65ef9428029b822816d21d315e675db4f84557c99a95453842`) | Git LFS |
| `xapk/UnityDataAssetPack.apk` | 187 MB | Split APK containing Addressables asset bundles | Git LFS |
| `xapk/com.zilliongames.collectionidle.apk` | 48 MB | Base APK with DEX code and metadata | Plain Git |
| `xapk/config.arm64_v8a.apk` | 45 MB | Architecture split containing native shared objects | Plain Git |
| `ext/data/assets/aa/Android/defaultlocalgroup_assets_all_*.bundle` | 130 MB | Addressables bundle containing all character/texture assets | Git LFS |
| `ext/native/lib/arm64-v8a/libil2cpp.so` | 112 MB | Compiled IL2CPP game binary | Git LFS |
| `ext/base/` | 122 MB | Unpacked base APK resources | Plain Git |
| `ext/native/` | 39 MB | Remaining native `.so` files | Plain Git |

## Setup & Cloning

To clone with full binary payloads:
```bash
git clone https://github.com/v-reza/switchingheroes-raw.git
cd switchingheroes-raw
git lfs pull
```
