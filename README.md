# Z Creative Asset Critique Skill

This repository is the authoritative technical source for the `z-creative-asset-critique` skill. The skill gives agents a quick, practical way to review creative assets without making ordinary VA work feel like a formal design audit.

## Purpose and When to Use

Use this skill when a user needs feedback on a marketing graphic, photograph, social post, ad, logo, wordmark, hero image, offer sheet, or other text-heavy visual. It begins with a short Quick Look and adds a Focus Review or Pre-Flight Review only when the requester asks or the asset has a specific, high-impact concern.

The authoritative runtime instructions are in [SKILL.md](SKILL.md). The three reference files provide only the deeper checks that an agent needs on demand: asset-type checks, channel and production boundaries, and concise response patterns.

## Do Not Use

Do not use this skill to create or edit graphics, publish an asset, log into Canva, certify legal or trademark rights, approve print production, or claim that technical checks such as dimensions, file size, links, QR codes, or final exports passed without evidence. The skill reports visible findings and identifies the responsible next step when a separate capability is required.

Do not use the skill as a numerical scoring system or a universal accessibility, legal, conversion, or brand audit. It must preserve working design choices and avoid creating unnecessary revision rounds.

## Validation and Deployment

Validate this repository with the bundled ZedBiz AI skill-developer validator:

```bash
python3 /path/to/z-ai-skill-developer-Skill/scripts/validate_skill.py --repository /path/to/z-creative-asset-critique
```

Run the manual happy-path review in [tests/happy-path.md](tests/happy-path.md) before deployment. For OpenClaw, place the skill in the confirmed skills root, run `openclaw skills list`, and test it in a fresh session. Do not assume a local path, discovery result, or restart procedure without checking the target runtime.

## Safety and Approval Boundaries

The skill contains no secrets and must never request, store, or expose credentials, tokens, keys, or complete environment files. It does not grant authority to alter source files, publish assets, access a paid service, or make a production change.

A human owner must approve any asset editing, publishing, paid production, client delivery, or other production-impacting action. GitHub is the authoritative source for the technical skill files. The detailed operating SOP belongs in Notion and must link back to this repository rather than become a competing executable copy.

