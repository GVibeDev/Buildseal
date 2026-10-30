# Changelog

## 0.3.1 — 2026-10-30

- Correct the GCM wording: a fresh unique nonce can be used with the same key, within usage limits.
- Make the Standard path without Runtime Guard explicit in objectives, diagram and adapter responsibilities.
- Distinguish logical release identity from individually signed distribution variants; declare the remaining format and correspondence checks as open.
- Bind attestation references to signed expected digests and require signer/subject verification without circular manifest references.
- Replace ambiguous certification terminology and clarify that preserved numbering does not preserve all heading anchors.
- Apply the corrections in Italian and English; LICENSE remains unchanged. No software or benchmark results introduced.

Correzioni documentali bilingui: nonce GCM, Guard opzionale, identità di release e varianti, verifica delle attestazioni e terminologia. Nessuna modifica alla licenza o risultato sperimentale.

## 0.3 — 2026-10-30

Documentation revision following external technical review. No implementation or benchmark results are introduced. Existing report filenames and section numbering 1–14 are preserved; headings and their generated anchors may change. Sections 15–17 are added. The LICENSE file is unchanged.

### Changes

- Refocus the abstract and README on release identity, provenance and integrity; keep anti-extraction optional and experimental.
- Rewrite section 5: key origin/delivery, signing versus encryption keys, compromise scope, HKDF context, AEAD versus signatures, nonce lifecycle and Connected boundaries.
- Treat code/manifest key-entanglement as a comparative hypothesis rather than a trust root.
- Add static extraction, dynamic dumps, loader patching, marker collusion/transplantation and extractor reuse to the assessment.
- Add native-engine controls, extraction coverage/fidelity, patch bytes, staging and developer diversification costs to the experiments.
- Move media work outside the BuildSeal validation plan; retain only provenance interoperability boundaries.
- Add channel-specific adoption hypotheses, primary-source related work and future component-licensing questions.

### Still open

PoC target and thresholds; production key delivery; algorithms and nonce allocation; packaging granularity; independent verification/bootstrap; measurable advantage over existing tools; store compatibility; future component licensing and actual adopter demand.

## 0.3 — Italiano

Revisione documentale in seguito a una review tecnica esterna. Nessun risultato sperimentale o software introdotto. Nomi dei report e numerazione 1–14 conservati; aggiunte sezioni 15–17. LICENSE invariata.

- Chiariti posizionamento, gestione delle chiavi, firme, AEAD, nonce e limiti di Connected.
- Key-entanglement mantenuto come ipotesi da confrontare, non radice di fiducia.
- Aggiunti dump dinamico, patch del loader, collusione/trapianto dei marcatori e riutilizzo degli estrattori.
- Rafforzati confronti con le protezioni native, metriche di copertura/fedeltà e costi di patch, staging e diversificazione.
- Ricerca media separata; aggiunte matrice di adozione, related work e decisioni sulle licenze future.
- Restano aperti target e soglie del PoC, gestione delle chiavi in produzione, granularità, bootstrap, vantaggio misurato, compatibilità, licenze e domanda reale.

## 0.2 — 2026-10-30

Initial bilingual feasibility proposal published for technical peer review. / Prima proposta bilingue di fattibilità pubblicata per revisione tecnica.
