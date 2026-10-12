# Assets.MadeHuman

Portable MadeHuman conversions of the MIT-licensed Microsoft Rocketbox corpus.
The exact Microsoft source revision, converter revision, source/output hashes,
license and runtime URL are recorded per artifact in `catalog.json` and in the
adjacent `*.rocketbox.json` sidecar.

- Avatars: `0` ready of `0` sources
- Animations: `0` ready of `0` sources
- Garments: `3` ready of `3` reviewed harvests
- Invalid or missing: `0`

`Avatars/` and `Animations/` are a Git-LFS-ready release mirror.  Production
serving does not depend on Git LFS: Seeker serves the canonical external asset
store and the netdisk is its durable backup.  Regenerate this directory with
`tools/blender/pipeline/build_rocketbox_release.py`; do not hand-edit hashes.

Garments harvested from these avatars are intentionally separate.  A candidate
must be an edge-connected source-topology component, retain UV/material
provenance, pass a no-skin semantic review, and pass the existing try-on visual
gates before it can enter the wardrobe catalog.
