# Spam Risk Reviewer Delivery Report

- Package: spam-risk-reviewer@0.1.0
- PR: 
https://github.com/runxhq/runx/pull/146
- Source: 
https://github.com/Li-AmG/spam-risk-reviewer-skill
- Raw X.yaml: 
https://raw.githubusercontent.com/Li-AmG/runx/e53329d2d58954060def38291d12a3c7f69d81fa/skills/spam-risk-reviewer/X.yaml
- Raw SKILL.md: 
https://raw.githubusercontent.com/Li-AmG/runx/e53329d2d58954060def38291d12a3c7f69d81fa/skills/spam-risk-reviewer/SKILL.md
- runx CLI version observed: runx-cli 0.6.13
- runx doctor: success with zero diagnostics
- Low-risk fixture: pass, preflight_clear true, no blockers
- High-risk fixture: hold, preflight_clear false, needs_human escalation
- Authentication checks: SPF, DKIM, DMARC are read from input and never invented
- List hygiene checks: bounce rate, complaint rate, freshness, warm-up days compared to fixed thresholds
- Effect boundary: public_send remains owned by governed send-as; this skill emits only send_risk_verdict
- Local runx receipt/harness blocker: Windows receipt store returned os error 87 despite signed env and explicit receipt dirs
- Public URL index blocker: api.runx.ai returned rate_limited with retry_after_seconds=1394; retry is queued by operator

- GitHub Actions harness status: passed
- GitHub Actions dogfood receipt_ref: runx:receipt:sha256:a975fab3a794701688ec6df10e5663084625f70e4fd6ccd1107f8b8e136ddc9b
- GitHub Actions verify status: unknown
