# MyLeadGenSecret AI Campaign Workflow

This repository holds the reusable assistant instructions for preparing and sending an MLGS affiliate email from Costas's connected Chrome session.

## Start a campaign

In ChatGPT Work Mode, provide the affiliate link. The assistant will check that Chrome has an authenticated MyLeadGenSecret mailing-system tab, research the offer, compose a short and persuasive message, choose a recent non-overlapping date cohort, place the affiliate link behind natural anchor text, preview the campaign, send it when the checks pass, and record the campaign result.

If the MLGS tab is missing or signed out, the assistant will ask you to open or reconnect it. Do not share your password or browser session data.

## Browser-driven, on-demand workflow

This is not a GitHub Actions mail sender. A GitHub-hosted runner cannot attach to the Chrome session you connect in ChatGPT, and the MLGS help material describes its built-in mailing system or downloading leads rather than a public sending API. The assistant uses the connected browser for the live MLGS interface.

## Audience rotation

The MLGS mailing page groups leads by signup date. The observed account page showed daily date groups of 100 leads. A first 9,000-lead campaign therefore needs 90 such groups; 12,000 needs 120. Selecting the newest 9,000 again tomorrow would repeat roughly 8,900 recipients. The assistant must track date ranges and avoid overlap; if a fresh non-overlapping cohort is unavailable, it must stop rather than resend to the same group.

The initial campaign defaults to 9,000. The assistant may choose 12,000 only when reported campaign results and offer relevance support scaling.

## Public repository and privacy

This repository is public. Keep only generic workflow instructions and blank templates here. Never commit lead addresses, IP addresses, passwords, browser cookies, session files, private affiliate links, or actual campaign results. Use the private campaign record in the current ChatGPT conversation and the ignored local log template when available.

See [AGENTS.md](AGENTS.md) and [docs/MLGS-CAMPAIGN-WORKFLOW.md](docs/MLGS-CAMPAIGN-WORKFLOW.md) for the complete operating rules.
