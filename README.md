Firmware update check URL: `GET` to `http://cdn.zinkapps.com/brother-secure-versions.js` (typically adds a timestamp to end to bust cache, eg: `http://cdn.zinkapps.com/brother-secure-versions.js?20220805181152`)

Files then appear to be at http://cdn.zinkapps.com/[filename]

`Latest Ver` is `YYYY-MM-DD-??`, where `??` is a build number? Or possibly always `02`.

Haven't figured out the .gpg extension decryption/decompression yet.

## Known firmware versions

- [`brotherupgrade-2021032102.tgz.gpg`](http://cdn.zinkapps.com/brotherupgrade-2021032102.tgz.gpg)
- [`brotherupgrade-2022061402.tgz.gpg`](http://cdn.zinkapps.com/brotherupgrade-2022061402.tgz.gpg)
- something dated 2019 which came preinstalled on my VC-500W but I forgot to record datestamp before upgrading, and my `wget` script isn't finding it

## Sniffing for versions

`wget http://cdn.zinkapps.com/brotherupgrade-{2019..2022}{01..12}{01..31}{01..05}.tgz.gpg `
