# Sign motion evaluation — rating instrument

A blinded rating instrument for a Thai Sign Language user study of computer-generated
sign-language skeleton motion. Participants watch short skeleton clips and rate the
motion on four five-point scales, then complete two paired-comparison phases.

- `index.html` — the complete instrument: markup, logic, styling and all 60 stimulus
  clips embedded as data URIs. No build step, no dependencies, and no network calls
  except to the one response endpoint configured inside it: answers are uploaded to it
  as they are given, and two read-only questions are asked of it — which participant
  numbers are already in use, and which of this session's rows it has received. Neither
  read returns an answer given by anybody.
- Stimuli are 178-keypoint skeleton renderings derived from pose estimates, not video
  of any person.

Participant responses are uploaded to an endpoint controlled by the researcher as they
are given, and are also kept in the browser's local storage on the participant's own
device, under their participant number. That copy is what makes a session resumable: an
evaluation interrupted on a phone can be continued on the same device from the clip it
stopped at, and anything the endpoint did not receive is sent the next time the same
link is opened there. No response is shared with, or visible to, other participants.

This page is published only so that study participants can open it without an account.
It is not a general-purpose tool and carries no licence to reuse the stimuli.
