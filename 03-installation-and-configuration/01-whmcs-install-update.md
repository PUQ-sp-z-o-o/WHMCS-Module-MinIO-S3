# WHMCS Installation and Update

### MinIO S3 module **[WHMCS](https://puqcloud.com/link.php?id=77)**
#####  [Order now](https://puqcloud.com/whmcs-module-minio-s3.php) | [Download](https://download.puqcloud.com/WHMCS/servers/PUQ_WHMCS-MinIO-S3/) | [Community](https://community.puqcloud.com/)

## System requirements

| Requirement | Minimum / Supported Version |
|-------------|----------------------------|
| **WHMCS** | 8.x+, 9.x+. |
| **PHP** | 7.4, 8.1, 8.2, 8.3, 8.4 |
| **ionCube Loader** | v15+ |
| **MinIO Server** | `RELEASE.2025-04-22T22:12:26Z` or lower |

> [!IMPORTANT]
> **MinIO Server Version:** The module works exclusively with MinIO server version **`RELEASE.2025-04-22T22:12:26Z`** or lower. Versions newer than this release are not supported.
>
> **ionCube Loader:** The module uses ionCube encoding. Make sure ionCube Loader is installed and active on your server.


---

## Download

> **Note:** The module now uses **ionCube 15**, which provides universal out-of-the-box support for all encodings across modern PHP runtimes.
>
> All versions can be found at this link:
> [https://download.puqcloud.com/WHMCS/servers/PUQ_WHMCS-MinIO-S3/](https://download.puqcloud.com/WHMCS/servers/PUQ_WHMCS-MinIO-S3/)
>
> Older module versions for WHMCS 8 are available in the archive directory:
> [https://download.puqcloud.com/WHMCS/servers/PUQ_WHMCS-MinIO-S3/archive/](https://download.puqcloud.com/WHMCS/servers/PUQ_WHMCS-MinIO-S3/archive/)

1. Download the latest version of the module directly to your server:
   ```bash
   wget https://download.puqcloud.com/WHMCS/servers/PUQ_WHMCS-MinIO-S3/PUQ_WHMCS-MinIO-S3-latest.zip
   ```

2. Unzip the archive:
   ```bash
   unzip PUQ_WHMCS-MinIO-S3-latest.zip
   ```

---

## Installation

### Upload files

Copy the `puqMinIOS3` directory from the extracted archive to the WHMCS servers module directory:

```bash
cp -r puqMinIOS3 /path/to/whmcs/modules/servers/
```

Or target path:
```
WHMCS_WEB_DIR/modules/servers/puqMinIOS3
```

Once the files are uploaded, proceed to the configuration chapter to set up your server and product.

---

## Update

The update procedure is the same as installation — replace the existing files with the new version:

1. Download the latest version as described in the Download section.
2. Unzip the archive.
3. Replace the existing `WHMCS_WEB_DIR/modules/servers/puqMinIOS3` directory with the new one.
4. Verify the version number in the module interface matches the new release.
