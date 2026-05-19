# Decision Report: Scribe Rail

A typed, EHR aware durability rail for AI scribe writes: every note enters a deterministic pipeline of transform -> validate -> write -> confirm -> reconcile with semantic fallback, and the clinician sees one sentence - never a lost session.

## Evidence-Grounded Findings

CLAIM: hinges policy boundary should `block release until replay is understood` because blocks=2 reviews=3 mean_severity=1.708. [EVID: ev_0033]
CLAIM: nextvisit drift should `block release until replay is understood` because blocks=2 reviews=3 mean_severity=2.5. [EVID: ev_0088]
CLAIM: nextvisit evidence recall should `block release until replay is understood` because blocks=3 reviews=3 mean_severity=1.875. [EVID: ev_0066]
CLAIM: value failure replay should `block release until replay is understood` because blocks=2 reviews=4 mean_severity=3.333. [EVID: ev_0110]
CLAIM: whole gap should `block release until replay is understood` because blocks=3 reviews=2 mean_severity=3.333. [EVID: ev_0011]
CLAIM: whole reviewer handoff should `block release until replay is understood` because blocks=2 reviews=4 mean_severity=2.583. [EVID: ev_0121]
