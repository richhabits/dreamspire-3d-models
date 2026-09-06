# DreamSpire 3D Models

Auto-generated product `.glb` files for DreamSpire AR / 3D spin.

## Hosting

Repo is **public**. Free CDN (preferred):

```
https://cdn.jsdelivr.net/gh/richhabits/dreamspire-3d-models@main/models/{product-handle}.glb
```

Raw GitHub also works:

```
https://raw.githubusercontent.com/richhabits/dreamspire-3d-models/main/models/{product-handle}.glb
```

No Git LFS — files are normal git blobs (~1–4 MB each).

## Naming

Filename stem == Shopify product `handle` (e.g. `dreamspire-classic-logo-unisex-t-shirt.glb`).
`test1.glb` is a scratch asset and is not wired to a product.

## App wiring

- Flutter resolves `ar.model_glb` metafield, else falls back to the CDN URL by handle.
- `sync_ar_metafields.js` in dreamspire-app writes metafields when a live Admin token is set.
