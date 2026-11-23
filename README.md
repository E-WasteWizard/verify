# verify

Encrypted lookup files for [e-wastewizard.com/verify](https://e-wastewizard.com/verify), served by GitHub Pages.

Each `c/<index>.json` holds one E-Waste Wizard Certificate of Destruction. The file name and its AES-GCM key come
from the certificate ID plus the manifest fingerprint printed on the certificate, so a file can only be found and
opened by someone holding that certificate. Inside is the certificate's Ed25519-signed verification code, which the
verify page then checks against E-Waste Wizard's public key. Files are published by NetScryer's ITAD module
(`ui/itad_lookup.py`); do not edit them by hand.
