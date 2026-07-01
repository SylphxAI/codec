# @sylphx/codec

## 1.1.1

### Patch Changes

- 1801180: Forward-fix published package dependency metadata so internal workspace dependencies are materialized from the current workspace versions during npm publication.

## 1.1.0

### Minor Changes

- d2120de: Add 48 new codec implementations

  **Image formats:**

  - AVIF, HEIC, JXL, BPG, FLIF (modern image formats)
  - DICOM (medical imaging)
  - CR2, NEF, ARW, DNG, ORF, RW2, RAF, PEF (RAW camera formats)
  - JP2/J2K (JPEG 2000)
  - XCF (GIMP)

  **Video formats:**

  - WebM, MOV, MPEG, 3GP, F4V, RM/RMVB, SWF, VOB, APNG, OGV

  **Audio formats:**

  - MP3, AAC, OPUS, AC3, DTS (common lossy)
  - WMA, APE, ALAC, TTA, TAK, WV, MPC (lossless/proprietary)
  - AMR, SPX (speech codecs)
  - M4A, MKA, CAF (containers)
  - DSF (DSD audio)
  - MOD, S3M, XM, IT (tracker formats)

  Total: 101 codecs, 2328 tests, 97M+ assertions

### Patch Changes

- cc6960e: Forward-fix published package metadata so workspace protocol dependencies are materialized during npm publication.
- Updated dependencies [d2120de]
- Updated dependencies [cc6960e]
  - @sylphx/codec-core@1.0.1
