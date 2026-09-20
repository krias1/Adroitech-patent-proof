# Privacy-safe asset provenance review — f0051f31731f990067ad4776a2eaef62eef7c376

## Source boundary

Canonical source: `krias1/Adroitech-Logic-Core`

Commit: `f0051f31731f990067ad4776a2eaef62eef7c376`

Path: `AdroitechLogic/Run Receipts/2026-08-29_AUGUST_2026_MONTH_END_CONTINUITY_SYNC.md`

Git blob SHA-1: `428c53a28e1c9e66c76bc98502dc683fe5b20811`

Commit timestamp UTC: `2026-08-29T22:25:48Z`

This public review deliberately omits serial numbers, IMEI/MAC values, credentials, private account information, exact private asset coordinates, purchase/payment details, and other identifiers that belong only in the separate private asset/capital-contribution reconstruction dataset.

## Asset/hardware evidence established by the committed checkpoint

The checkpoint materially references the following distinct hardware or physical-asset classes and therefore cannot be classified as `reviewed_no_asset_event`:

1. Main Intel Core i9-14900K / ASUS Z790 MAX GAMING WIFI7 tower used as the primary Proxmox/AI host.
2. NVIDIA Tesla P40 24 GB compute GPU assigned to the Huey VM rather than the physical Windows workstation VM.
3. Multiple storage devices/classes backing HueyCore, AI/model storage, hot VM storage, NAS/scratch storage, and quick-deploy/service storage.
4. Physical Windows workstation integration using Intel UHD 770 graphics, Intel XHCI USB, and Intel HDA passed through from the host into VM104.
5. Removable 128 GB `ADROITECH_FIELD` service-library media and a separate durable quick-deploy warehouse.
6. Ubiquiti UniFi Mobile Router Industrial, model `UMR-Industrial-US`, used in the T-Mobile Business edge architecture. Sensitive device identifiers are intentionally withheld here.
7. Dell Wyse 5020 / Dx0Q repurposing path, including referenced SK hynix memory, Apacer SATA storage, Hitachi 2.5-inch SATA HDD, SK hynix PC711 NVMe, and an M.2-to-SATA adapter. The source does not by itself establish accounting ownership or contribution treatment for every component.
8. Samsung Galaxy Tab S9 FE 5G, model `SM-X518U`, used as an operator-control endpoint.
9. Camera/NVR equipment classes including Tapo and ONVIF/RTSP cameras plus dedicated DVR/NVR storage.
10. Field-service and embedded-development hardware families referenced through the service library, including Pico/ESP, JTAG/SWD, NFC/RFID/Proxmark, serial, SPI/I2C/EEPROM, CAN/OBD and related diagnostic interfaces. A library reference is not evidence that every possible device in a family was owned.
11. Public-edge and LAN infrastructure referenced through the Golden node, NAS, WireGuard endpoints, and downstream office/network peripherals.

## Evidence classification

- `verified`: Git commit identity, changed path, Git blob identity, commit timestamp, and the fact that the committed checkpoint contains these hardware references.
- `source_stated`: configuration, deployment state, observed device state, model identity, component identity, and historical events described inside the checkpoint unless independently corroborated by an earlier/later Git artifact.
- `derived`: classification of the above references into normalized asset/hardware families for reconciliation.
- `inference`: none promoted to fact in this public record.
- `needs_reconciliation`: physical identity matching across earlier/later mentions; acquisition source/date; purchase amount; taxes/shipping/fees; payer/entity; personal-versus-company ownership; contribution/reimbursement/loan status; placed-in-service date; disposal/return state; warranty/receipt linkage; and exact private identifiers where the private ledger has not yet independently reconciled them.

## Capital-contribution/accounting boundary

The checkpoint proves business/project use references for multiple physical assets. It does **not**, by itself, prove purchase price, fair-market value, tax basis, depreciation treatment, legal ownership, or that any personally owned item was contributed to a business. Those fields remain private-ledger reconciliation questions and must be tied to receipts, payment evidence, inventory records, and explicit ownership/contribution records before being marked verified.

## Predecessor targets

The checkpoint itself points to predecessor evidence that should be traversed before first-origin claims are assigned, including the VM104 physical-workstation session receipt, the UMR live identity/acceptance record, quick-deploy tool-shelf manifests/helpers, prior Golden/WireGuard/Huey/Frigate records, and earlier inventory/asset records.

## Reproducibility

1. Fetch commit `f0051f31731f990067ad4776a2eaef62eef7c376` from `krias1/Adroitech-Logic-Core`.
2. Verify the changed path and Git blob `428c53a28e1c9e66c76bc98502dc683fe5b20811`.
3. Inspect the hardware/infrastructure sections of the checkpoint.
4. Reconcile each physical item against dedicated inventory records and predecessor commits before merging identities.
5. Keep sensitive identifiers and financial/accounting fields in the private asset dataset, not this public proof repository.

This record establishes the existence of hardware/asset references and their architectural roles at this Git state. It makes no unsupported legal, tax, valuation, ownership, inventorship, or priority conclusion.