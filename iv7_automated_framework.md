# iV7 Automated Truth-Backfill Framework

Purpose: records-integrity pipeline for tracking public statements about War Powers Resolution notifications and related policy claims. Scope is documentation and audit logging only.

## Pipeline
1. Ingest public statements
2. Normalize to canonical claim records
3. Detect drift vs archived evidence
4. Map evidence chain
5. Backfill corrected timeline
6. Score risk (CD, CL, AR, SIS, BII)

## State Model
- STABLE: consistent with evidence
- UNSTABLE: conflict detected
- MAPPING: evidence collection in progress
- BACKFILLED: contradiction resolved with linked references
- RESIDUAL: historic conflict remains searchable

## BDS Compliance Minimum Metadata
claim_id, speaker, statement_text, statement_time_utc, ingest_time_utc, source_url, source_hash, evidence_links, state, confidence, jurisdiction, version
