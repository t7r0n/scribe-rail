# Failure Matrix: Scribe Rail

| Scenario | Failure mode | Metric | Gate | Evidence |
| --- | --- | --- | --- | --- |
| nextvisit evidence replay | nextvisit_drift | nextvisit_coverage | block release until cited evidence is regenerated | ev_0000 |
| hinges operator packet | hinges_blindspot | hinges_latency | accept only if decision claims cite fixture evidence | ev_0007 |
| hinges operator packet | hinges_blindspot | hinges_latency | accept only if decision claims cite fixture evidence | ev_0011 |
| value regression harness | value_misroute | value_precision | open a regression issue with trace and benchmark delta | ev_0014 |
| whole boundary probe | whole_gap | whole_risk | route to reviewer with evidence packet | ev_0021 |
| value regression harness | value_misroute | value_precision | open a regression issue with trace and benchmark delta | ev_0022 |
| nextvisit evidence replay | nextvisit_drift | nextvisit_coverage | block release until cited evidence is regenerated | ev_0028 |
