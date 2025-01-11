# server-platform-app-templates

This is a collection of templates for community app repositories on popular ecosystems, like Unraid, TrueNAs, CasaOS, etc.

## CasaOS

Users on CasaOS can install RomM via the [Big Bea CasaOS App Store](https://community.bigbeartechworld.com/).

### Updating the Big Bear repository

Update the files in the `casaos` directory in this repository for the latest version of RomM, making sure to update any env variables or other configuration settings. Then fork and clone the [Big Bear repository](https://github.com/bigbeartechworld/big-bear-casaos) to your local machine, and copy the contents of the `casaos` directory to the `/Apps/romm` directory in the Big Bear repository. Lastly open a PR to the Big Bear repository with the changes.

## Portainer

RomM is made available to Portainer users through [xeno1's Portainer Templates](https://github.com/xneo1/portainer_templates). Follow the [instructions in the README](https://github.com/xneo1/portainer_templates?tab=readme-ov-file#installing) to add the templates to your Portainer instance.

### Updating xeno1's repository

Update the files in the `portainer` directory in this repository for the latest version of RomM. Consult the [Portainer App Template Docs](https://docs.portainer.io/2.19/advanced/app-templates/format) for more information on how to format the template. Then fork and clone xeno1's repository above to your local machine, update `template.json` is required, and copy `/portainer/Stack/romm.yml` to `Template/Stack/romm.yml`. Lastly open a PR to xeno1's repository with the changes.

## Unraid

The template for Unraid is hosted in another repository, [rommapp/unraid-templates](https://github.com/rommapp/unraid-templates), since it's made available through the [Community Apps plugin](https://forums.unraid.net/topic/38582-plug-in-community-applications/).

## TrueNAS

TrueNAS users can install RomM through the official [TrueNAS App Catalog](https://github.com/truenas/apps).

### Updating the TrueNAS Apps Catalog repository

The format expected by TrueNAS Apps Catalog (TNAC) is delicate and prone to errors, so be extra careful when updating any files under `/truenas`. You can consult other entries in the TNAC repository for guidance. Once you've updated the files in the `truenas` directory in this repository, fork and clone the TNAC repository to your local machine, and copy the contents of the `truenas` directory to the `/ix-dev/community/romm` folder in the TNAC repository. Lastly open a PR to the TNAC repository with the changes.

## HexOS

HexOS apps are pulled from the TrueNAS Apps Catalog, so no additional steps are required to make RomM available on HexOS.

## Synology

Packages for Synology are generated by [spksrc](https://github.com/SynoCommunity/spksrc), a cross compilation framework to create native packages for the Synology's NAS. At this time, the package for RomM is not available in the SynoCommunity repository.
