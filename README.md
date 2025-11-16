# BREVOS – Bharat Real-Estate Valuation Open Standard

BREVOS is an open, India-native data standard for structuring residential and commercial real-estate valuations.

It provides a common, machine-readable language for:

- Banks and HFCs  
- NBFCs and alternative lenders  
- Insurers  
- Registered valuers and valuation firms  
- AVM / AI-powered valuation platforms  
- Proptechs, marketplaces, and regulators  

BREVOS is inspired by international efforts such as UAD 3.6, but is designed from the ground up for India's legal diversity, documentation styles, and data constraints.

---

## Goals

- **Standardise** how valuation data is captured and exchanged in India  
- **Enable automation** of underwriting, risk scoring, and audit trails  
- **Support AVMs and AI agents** with clean, structured inputs  
- **Reduce friction** between valuers, lenders, and technology platforms  
- **Remain open and extensible** via state-level and sector-level extensions  

---

## Domains

BREVOS 1.0 defines five core domains:

1. **BREVOS-ID (`id_domain`)** – identity of property, valuer, assignment  
2. **BREVOS-LG (`legal_domain`)** – title, encumbrances, approvals, dues  
3. **BREVOS-PC (`physical_domain`)** – land, building, condition, amenities, deviations  
4. **BREVOS-MR (`market_domain`)** – guideline value, AVM, comparables, liquidity  
5. **BREVOS-RX (`risk_domain`)** – risk scores, grades, overvaluation probability, FSD  

Plus supporting sections:

- `assignment` – loan/engagement context  
- `evidence` – links and hashes for documents, photos, and maps  
- `audit` – workflow and digital signing  
- `state_extension` – fields specific to individual states (KA, MH, TN, UP, etc.)

---

## Schema

The canonical JSON Schema for BREVOS 1.0 lives at:

- `schema/brevos-valuation-1.0.json`

The schema is written in JSON Schema draft-07 and is designed to be:

- strict enough for lender ingestion  
- flexible enough for different asset types and workflows  

---

## Example

A complete sample valuation JSON is available in:

- `examples/valuation-apartment-ka-1.json`

---

## Versioning

BREVOS uses semantic versioning:

- **MAJOR** – breaking changes  
- **MINOR** – backward-compatible additions  
- **PATCH** – clarifications and non-breaking fixes  

The current version is: **1.0.0**.

---

## Governance

BREVOS is governed by a neutral, open working group that includes:

- Registered valuers  
- Banks / HFCs / NBFCs  
- Insurers  
- Technology and data providers  
- Independent domain experts  

Change proposals follow an RFC process. See:

- `GOVERNANCE.md`  
- `RFCs/` directory  

---

## Implementations

Early implementations include:

- AVM / valuation platforms  
- Lender-side ingestion pipelines  
- Valuer field apps  

To add your implementation, open a pull request to `IMPLEMENTATIONS.md`.

---

## Contributing

We welcome contributions from valuers, lenders, engineers, and researchers.

1. Review the existing schema  
2. Check open issues and RFCs  
3. Propose changes via a GitHub Issue or RFC PR  

See `CONTRIBUTING.md` for detailed guidelines.

---

## License

The BREVOS specification and reference schemas are made available under the **Apache 2.0 License**.

See `LICENSE` for details. You can contact on valuemind[dot]co[at]gmail[dot]com
  
