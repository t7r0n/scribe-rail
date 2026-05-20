# Scribe Rail

A typed, EHR aware durability rail for AI scribe writes: every note enters a deterministic pipeline of transform -> validate -> write -> confirm -> reconcile with semantic fallback, and the clinician sees one sentence - never a lost session.

![Scribe Rail working dashboard](outputs/project_working.svg)

## Why it exists

Nextvisit's whole value prop hinges on ambient transcription -> structured note working reliably across nine EHRs and HL7/FHIR.

Most internal demos stop at a pretty chart. This repository is built around the harder part: a repeatable path from fixture, to failure, to evidence, to the operator action a serious team would actually trust.

## What is inside

- A deterministic replay harness tuned around nextvisit, whole, and value.
- Company-specific strategy code in `src/scribe_rail/strategy.py`, not just README-level customization.
- Citation-locked reports where every decision claim has to point back to a generated evidence ID.
- Two visual artifacts generated from the latest run: `outputs/project_working.svg` and `outputs/evidence_map.svg`.
- A portable demo pack with JSON, CSV, Markdown, HTML, SVG, and benchmark artifacts.

![Scribe Rail evidence map](outputs/evidence_map.svg)

## Signals it measures

- `nextvisit coverage`
- `whole risk`
- `value precision`
- `hinges latency`

## Failure modes it plants

- nextvisit drift
- whole gap
- value misroute
- hinges blindspot

## Run it locally

```bash
uv sync
uv run scribe-rail all
uv run pytest -q
uv run ruff check .
```

## Outputs worth opening

- `outputs/dashboard.html`
- `outputs/project_working.svg`
- `outputs/evidence_map.svg`
- `outputs/operator_brief.md`
- `outputs/decision_report.md`
- `outputs/strategy_model.json`
- `outputs/demo_pack.zip`

## Sources

- https://news.nextvisit.ai/
- https://www.barchart.com/story/news/36340110/nextvisit-ai-announces-launch-of-groundbreaking-behavioral-health-documentation-platform
- https://aijourn.com/nextvisit-ai-announces-launch-of-groundbreaking-behavioral-health-documentation-platform/
- https://github.com/yannelli
- https://ryanyannelli.com
- https://github.com/yannelli/attempt
- https://www.crunchbase.com/organization/nextvisit

## Boundary

Everything runs locally against synthetic fixtures. There are no credentials, no customer records, no outreach files, and no hosted API dependency.
