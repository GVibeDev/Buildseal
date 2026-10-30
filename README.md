# BuildSeal

**Release identity, provenance and integrity for indie games — a proposal for technical peer review.**

**Identità, provenienza e integrità delle release indie — proposta per revisione tecnica.**

## Read the reports / Leggi i report

| Language / Lingua | Document / Documento |
|---|---|
| English | [Abstract and technical feasibility report](BuildSeal_Report_EN.md) |
| Italiano | [Abstract e rapporto tecnico di fattibilità](BuildSeal_Report_IT.md) |

**Status / Stato:** pre-development proposal, report version 0.3.1, 30 October 2026. No prototype or benchmarks yet. / Proposta pre-sviluppo, report versione 0.3.1, 30 ottobre 2026. Nessun prototipo o benchmark ancora disponibile.

## English

BuildSeal explores how official game releases can be identified, verified and managed throughout their lifecycle, from a candidate build to a published baseline, patch or hotfix.

The proposed architecture combines an engine-independent Core with engine-specific adapters. It covers signed manifests, cryptographic file digests, layered project/release/distribution identities, provenance attestations and verifiable update lineage. An experimental protection profile would add a Runtime Guard and selective encryption of resources required by the game.

The goal is to detect tampering, reject inconsistent release components in the official loading and update paths, improve forensic traceability and measure whether additional protection raises the cost of opportunistic abuse. A fully attacker-controlled client remains a fundamental limitation: BuildSeal does not claim unbreakable DRM or prevention of independent reconstruction from gameplay footage.

Media provenance and watermarking belong to **separate research**. Preventing reconstruction from screenshots or video is outside BuildSeal's protection scope. Protected remains an optional experiment; no improvement over native engine protection has yet been demonstrated.

### Purpose of this repository

This repository contains the proposal for technical peer review before implementation. Reviewers are invited to challenge the threat model, identify bypasses and operational costs, suggest existing standards to reuse and propose minimal experiments that could falsify the assumptions. See section 12 of either report for the review questions.

The reports discuss TUF, in-toto, SLSA, Sigstore and C2PA as possible foundations or references; no implementation or standards conformance is claimed.

## Italiano

BuildSeal esplora come identificare, verificare e gestire le release ufficiali di un videogioco lungo il loro ciclo di vita, dalla build candidata alla pubblicazione di baseline, patch e hotfix.

L'architettura proposta combina un Core indipendente dal motore con adapter specifici. Comprende manifest firmati, impronte crittografiche dei file, identità multilivello di progetto/release/distribuzione, attestazioni di provenienza e una genealogia verificabile degli aggiornamenti. Un profilo sperimentale aggiungerebbe un Runtime Guard e la cifratura selettiva di risorse necessarie al gioco.

L'obiettivo è rilevare alterazioni, rifiutare componenti di release incoerenti nei percorsi ufficiali di caricamento e aggiornamento, rafforzare la tracciabilità forense e misurare se le protezioni aggiuntive aumentino il costo degli abusi opportunistici. Il controllo completo del client da parte dell'attaccante resta un limite fondamentale: BuildSeal non promette DRM inviolabile né di impedire una ricostruzione indipendente da video di gameplay.

Provenienza dei media e watermark appartengono a una **ricerca autonoma**. Impedire la ricostruzione da screenshot o video è fuori dall'ambito di protezione di BuildSeal. Protected resta un esperimento opzionale: non è ancora dimostrato un vantaggio rispetto alle protezioni native dei motori.

### Scopo del repository

Questo repository raccoglie la proposta per una revisione tecnica prima dell'implementazione. Si invita a mettere alla prova il modello di minaccia, individuare bypass e costi operativi, suggerire standard esistenti da riutilizzare e proporre esperimenti minimi capaci di smentire le ipotesi. Le domande per i revisori si trovano nella sezione 12 di entrambi i report.

I documenti discutono TUF, in-toto, SLSA, Sigstore e C2PA come possibili basi o riferimenti; non dichiarano implementazioni o conformità a tali standard.

## License / Licenza

See [LICENSE](LICENSE) for the GNU General Public License v3.0 included in this repository. / Consulta [LICENSE](LICENSE) per la GNU General Public License v3.0 presente nel repository.

## Revision 0.3 / Revisione 0.3

This revision clarifies key management and trust boundaries, adds native-engine baselines, dynamic extraction and cross-copy attacks, and includes adoption, licensing and patch-size tradeoffs. Technical feasibility and user demand remain to be validated. See [CHANGELOG.md](CHANGELOG.md).

La revisione chiarisce gestione delle chiavi e confini di fiducia, introduce confronti con i motori, estrazione dinamica e attacchi tra copie e aggiunge adozione, licenze e costi delle patch. Fattibilità tecnica e domanda restano da verificare. Vedi [CHANGELOG.md](CHANGELOG.md).

### Corrections 0.3.1 / Correzioni 0.3.1

Clarifies key–nonce uniqueness, optional runtime protection, logical releases versus distribution variants, and authenticated attestation references. / Chiarisce unicità chiave–nonce, protezione runtime opzionale, release logiche e varianti distribuite, e riferimenti autenticati alle attestazioni.
