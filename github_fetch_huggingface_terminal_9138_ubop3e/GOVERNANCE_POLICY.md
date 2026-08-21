# External Dataset Licensing Policy

Every external dataset must be classified before it may be onboarded for production use.

## License classification

- **APPROVED** — Permissive licenses that allow commercial use, modification and
  redistribution without copyleft obligations. Approved license identifiers:
  `mit`, `apache-2.0`, `bsd-2-clause`, `bsd-3-clause`, `cc0-1.0`, `unlicense`.

- **REJECTED** — Copyleft / share-alike / non-commercial licenses that impose
  restrictions on derivative works. Rejected license identifiers:
  `cc-by-sa-3.0`, `cc-by-sa-4.0`, `gpl-*`, `agpl-*`, `lgpl-*`, `cc-by-nc-*`.

- **NEEDS_REVIEW** — Any dataset whose license is `other`, `unknown`, `custom`,
  missing, or otherwise not clearly identified must be flagged for manual legal
  review before it may be used.

## Decision rules (highest priority first)

1. If the declared license is in the APPROVED list -> **APPROVED**.
2. Else if the declared license is in the REJECTED list -> **REJECTED**.
3. Else -> **NEEDS_REVIEW**.

## Notes

- The license reported by the dataset hub metadata is authoritative.
- Always confirm the license by reading the dataset card/readme.
