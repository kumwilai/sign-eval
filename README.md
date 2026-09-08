# Sign motion evaluation — rating instrument

A blinded rating instrument for a Thai Sign Language user study of computer-generated
sign-language skeleton motion. Participants watch short skeleton clips and rate the
motion on four five-point scales, then complete two paired-comparison phases.

- `index.html` — the complete instrument: markup, logic, styling and all 60 stimulus
  clips embedded as data URIs. No build step, no dependencies, no network calls except
  the response upload endpoint configured inside it.
- Stimuli are 178-keypoint skeleton renderings derived from pose estimates, not video
  of any person.

Participant responses are uploaded to an endpoint controlled by the researcher and are
also retained in the browser's local storage as a fallback. No response is shared with,
or visible to, other participants.

This page is published only so that study participants can open it without an account.
It is not a general-purpose tool and carries no licence to reuse the stimuli.
