# BREVOS Governance Charter

## 1. Purpose

The Bharat Real-Estate Valuation Open Standard (BREVOS) exists to provide an open, interoperable and India-native data standard for real-estate valuations.

This charter defines how BREVOS is evolved, versioned, and maintained.

---

## 2. Principles

1. **Openness** – Participation is open to all affected stakeholders.  
2. **Neutrality** – No single organisation or vendor controls the standard.  
3. **Practicality** – Changes are grounded in real lender–valuer–platform workflows.  
4. **Backward Compatibility** – Breaking changes are rare and clearly signposted.  
5. **Transparency** – Discussions, decisions, and roadmaps are public by default.  

---

## 3. Roles

### 3.1 BREVOS Steering Committee (BSC)

- 5–9 members representing:
  - Valuers
  - Lenders (banks, HFCs, NBFCs)
  - Insurers
  - Technology providers
  - Independent experts  

Responsibilities:

- Maintain the official roadmap  
- Approve new major/minor versions  
- Resolve disputes on conflicting proposals  

### 3.2 Domain Working Groups (DWG)

Each core domain (ID, Legal, Physical, Market, Risk) may have a DWG.

Responsibilities:

- Draft domain-specific changes  
- Review state-level extensions  
- Provide implementation guidance  

### 3.3 Contributors

Anyone submitting issues, RFCs, or PRs to the repository.

Responsibilities:

- Provide clear, reproducible examples  
- Declare conflicts of interest where relevant  

---

## 4. Change Process

### 4.1 Issue

All proposed changes begin as a GitHub Issue tagged with:

- `domain:legal`, `domain:market`, etc.  
- `type:bugfix`, `type:extension`, or `type:breaking`  

### 4.2 RFC

Non-trivial changes require an RFC in `RFCs/` with:

- Problem statement  
- Affected stakeholders  
- Proposed change (schema diff)  
- Migration considerations  
- Test cases / examples  

### 4.3 Review and Voting

- DWGs review RFCs and recommend one of:
  - Accept
  - Accept with modifications
  - Defer
  - Reject  
- The BSC takes final decisions for MINOR and MAJOR versions by simple majority.

---

## 5. Versioning

BREVOS uses semantic versioning: `MAJOR.MINOR.PATCH`.

- **MAJOR** – changes that break backward compatibility  
- **MINOR** – new features and fields, backward compatible  
- **PATCH** – documentation, clarifications, default values  

The BSC publishes a changelog for every release.

---

## 6. State Extensions

State extensions (e.g. KA, MH, TN, UP) follow these rules:

- Must not change core semantics  
- Should only add fields or narrower enums  
- Must be documented in `extensions/<state>/`  
- Should include at least one complete example  

---

## 7. Conflict of Interest

Members of the BSC and DWGs must disclose:

- Commercial stakes in implementations  
- Direct regulatory or supervisory roles  

Where a conflict exists, the member abstains from voting on the affected change.

---

## 8. Dissolution and Forks

If the BSC becomes inactive for 12+ months, the community may:

- Elect a new BSC, or  
- Fork the standard under a new name, retaining the Apache 2.0 license terms  

BREVOS documentation and schemas remain under open license.

---

## 9. Contact

- Public issues: GitHub Issues  
- Security or compliance concerns: `security@brevos.org` (TBD)  
