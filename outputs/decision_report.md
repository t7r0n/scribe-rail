# Decision Report: Scribe Rail

A typed, EHR aware durability rail for AI scribe writes: every note enters a deterministic pipeline of transform -> validate -> write -> confirm -> reconcile with semantic fallback, and the clinician sees one sentence — never a lost session.

## Evidence-Grounded Findings

CLAIM: hinges operator packet should `accept only if decision claims cite fixture evidence` because blocks=4 reviews=5 mean_severity=2.556. [EVID: ev_0055]
CLAIM: nextvisit evidence replay should `block release until cited evidence is regenerated` because blocks=4 reviews=5 mean_severity=2.611. [EVID: ev_0044]
CLAIM: value regression harness should `open a regression issue with trace and benchmark delta` because blocks=3 reviews=5 mean_severity=2.528. [EVID: ev_0110]
CLAIM: whole boundary probe should `route to reviewer with evidence packet` because blocks=3 reviews=4 mean_severity=2.528. [EVID: ev_0077]
