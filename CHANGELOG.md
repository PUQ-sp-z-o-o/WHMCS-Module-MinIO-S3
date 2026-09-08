# Changelog

### MinIO S3 module **[WHMCS](https://puqcloud.com/link.php?id=77)**
#####  [Order now](https://puqcloud.com/whmcs-module-minio-s3.php) | [Download](https://download.puqcloud.com/WHMCS/servers/PUQ_WHMCS-MinIO-S3/) | [Community](https://community.puqcloud.com/)

---

## v4.0.0 (02-09-2026)

- Full compatibility with WHMCS 8.x and WHMCS 9+
- Universal **ionCube Loader v15** support for seamless encoding compatibility
- Modernized administrative product settings interface with dynamic injection and enhanced stability
- Improved client area responsiveness for bucket and storage management
- Enhanced API communication reliability and performance optimizations

---

## v3.1 (01-03-2026)

- Added null coalescing checks for all array and superglobal accesses to prevent "Undefined array key" warnings
- Added null-safe operators for object property access where object can be null
- Fixed type safety for typed class properties (preventing `TypeError` on null assignment)
- Added boundary checks for empty database query results

---

## v3.0 (25-01-2025)

- Support for WHMCS 9+
- Product module settings have been redesigned
- Updated client area interface design

> **Note:** Product reconfiguration is required after update.

---

## v2.0 (23-09-2024)

- Module coded with ionCube v15
- Supported PHP versions: 7.4, 8.1, 8.2
- Compatible with WHMCS 8.11.0+

---

## v1.9.1 (13-08-2024)

- Fixed bug with password, when "Show password" is "no"

---

## v1.9 (26-06-2024)

- Adapted to MinIO version RELEASE.2024-06-26T01-06-18Z

> **Note:** Module will not work with versions lower than this.

---

## v1.8 (06-06-2024)

- Client area more adapted for mobile version
- Buttons for copying login and password added to client area

---

## v1.7 (16-05-2024)

- User blocking disabled after limit reached
- Policy switches to "Raw policy Disk limit" when exhausted
- Added functional buttons and policy management in admin area
- Added Recalculate Disk Space button for clients

> **Note:** Need to insert "Raw policy Disk limit" in product settings.

---

## v1.6 (21-12-2023)

**Fixed Issues:**
- Bug preventing policy deletion when account deleted
- Improved API error logging

**New Features:**
- Disable bucket creation by default
- Set default bucket suffix
- Disable password display by default
- "Show" button for passwords
- Plain text password display options

> **Note:** Save 'Module Setting' in products.

---

## v1.5 (18-12-2023)

- Support MinIO RELEASE.2023-12-14T18-51-57Z
- Minor client area changes

---

## v1.4 (11-10-2023)

- Support MinIO RELEASE.2023-10-07T15-07-38Z
- 25 language translations added (Arabic, Azerbaijani, Catalan, Chinese, Croatian, Czech, Danish, Dutch, English, Estonian, Farsi, French, German, Hebrew, Hungarian, Italian, Macedonian, Norwegian, Polish, Romanian, Russian, Spanish, Swedish, Turkish, Ukrainian)

---

## v1.3 (08-09-2023)

- Support MinIO RELEASE.2023-09-07T02-05-02Z

---

## v1.2 (05-03-2023)

- Support PHP 8.1 and PHP 7.4
- Support MinIO RELEASE.2023-02-22T18-23-45Z
- Template changes with icons added
- API timeout set to 30

---

## v1.1 (22-02-2023)

- Support WHMCS V8.6
- Support PHP 8.1 (Loader v12) and PHP 7.4
- Template changes
- Service settings email template changed to dropdown
- Translations added: German, Ukrainian
- Updated deletion mechanism for objects, buckets, and users

---

## v1.0 (01-08-2022)

- First release
