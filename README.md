# GeoLite Update Repository for XC_VM

This repository is used by the XC_VM project to manage and distribute updates for the MaxMind GeoLite2 databases.

## Purpose

The repository contains scripts, archives, and documentation required to maintain and update the GeoLite2 database files (`.mmdb`) used by XC_VM.

## Integration with XC_VM

During the update process, XC_VM retrieves the required GeoLite2 files from this repository and installs them into the appropriate location where XC_VM services access geolocation data.

## Updating GeoLite2 Databases

1. Download the latest GeoLite2 City and/or ASN database package from MaxMind. A valid MaxMind account and acceptance of their license agreement may be required.
2. Upload the downloaded archive to this repository or run the provided update script (for example, `update_geolite.sh`) to automatically extract and replace the existing `.mmdb` files.
3. Verify the updated databases in a local or staging environment before deploying them to production.
4. Commit the updated files and create a pull request or merge the changes into the branch used by XC_VM.

## Licensing

GeoLite2 databases are provided by MaxMind and are subject to MaxMind's licensing terms. Ensure that any download, usage, or redistribution complies with the applicable license agreement.

## Support

For questions regarding integration, automation, or update procedures, please refer to the XC_VM documentation or contact the XC_VM maintainers.
