# meta-mender-toradex-nxp

Mender integration layer for Toradex family of boards.

The supported and tested boards are:

- Toradex Verdin iMX8M Mini
- Toradex Verdin iMX8M Plus
- Toradex Colibri iMX8X

## Dependencies

This layer depends on:

```
URI: https://git.toradex.com/meta-toradex-bsp-common.git
branch: scarthgap-7.x.y
revision: HEAD
```

```
URI: https://git.toradex.com/meta-toradex-nxp.git
branch: scarthgap-7.x.y
revision: HEAD
```

```
URI: https://github.com/mendersoftware/meta-mender.git
layers: meta-mender-core
branch: scarthgap
revision: HEAD
```

## Quick start

See the top level [README](../README.md) for instructions to build using the `kas` tool. Supported configurations are:

- [`verdin-imx8mm.yml`](../kas/verdin-imx8mm.yml)
- [`verdin-imx8mp.yml`](../kas/verdin-imx8mp.yml)  
- [`colibri-imx8x.yml`](../kas/colibri-imx8x.yml)

### Example build commands

```bash
mkdir -p meta-mender-community/mender-toradex && cd meta-mender-community/mender-toradex

# Build for Verdin iMX8M Mini
kas build ../kas/verdin-imx8mm.yml

# Build for Verdin iMX8M Plus
kas build ../kas/verdin-imx8mp.yml

# Build for Colibri iMX8X
kas build ../kas/colibri-imx8x.yml
```