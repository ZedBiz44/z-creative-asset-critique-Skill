# Happy-Path Acceptance Test

## Test Prompt

Provide a social graphic for a local home-service business. The graphic has a readable headline, relevant jobsite photo, clear offer, readable phone number, and no obvious visual defect. Ask: “Does this graphic work?”

## Expected Behaviour

The skill should use Quick Look without requiring a form. It should return a concise Ready or Visually ready verdict, identify at least one working element, avoid inventing a defect, and state only an evidence-based remaining check if one exists.

A suitable answer is:

> **Visually ready.** The headline is easy to spot, the jobsite photo supports the service message, and the offer is easy to scan. Keep the current layout. Confirm the final mobile export before treating it as fully ready.

## Pass Conditions

- The response does not demand a full creative brief.
- The response does not force a Focus Review merely because the asset is a social ad with text.
- The response does not invent a font, file-size, link, or platform-specification problem.
- The response does not add a change solely to appear helpful.
- The response distinguishes visible readiness from the untested final mobile export.

## Manual Record

Record the prompt, response, reviewer, date, and pass or fail result in the associated GitHub issue or pilot record when deployed to a live agent.

