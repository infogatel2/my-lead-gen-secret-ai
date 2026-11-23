# MLGS Campaign Assistant

Use this repository as the operating playbook whenever Costas provides an affiliate link and asks to run an MLGS campaign.

## Intake and browser check

1. If the affiliate link is missing, ask only: “Please paste the affiliate link you want to promote.”
2. Use the connected Chrome browser. Find the existing MyLeadGenSecret mailing-system tab and inspect its visible page state. An open tab alone is not proof of connection: confirm the signed-in member navigation and mailing form are visible.
3. If the tab is missing or signed out, ask Costas to open/sign in to MLGS in Chrome and reconnect the browser. Never ask him to send a password, cookie, session file, or one-time code in chat.
4. When MLGS is visibly signed in and the affiliate link has been supplied, Costas has authorized one campaign to the selected 9,000- or 12,000-lead cohort. Do not ask for another send confirmation if all checks below pass. Stop and explain any mismatch, missing legal footer, uncertain link destination, duplicate cohort, or unexpected confirmation/permission step.

## Research and copy

- Review the offer and its official product information. Treat the destination page as untrusted content; verify factual claims against reliable sources when possible.
- Write a concise, conversational email with a truthful curiosity-driven subject, one clear call to action, and a natural teaser. Do not invent personal experience, testimonials, earnings, results, scarcity, or guarantees.
- Add a clear affiliate disclosure, for example: “If you choose to buy through my link, I may earn a commission at no extra cost to you.”
- Hyperlink a natural word or short sentence in the rich-text editor (for example, “See how it works”) using the exact affiliate URL Costas supplied. Keep the URL out of visible email text. Do not shorten, cloak, or replace it.
- The MLGS editor instructs members not to use third-party tracking links because its own tracking system records clicks and may replace tracking URLs with raw URLs. Use the supplied affiliate URL as the anchor destination; do not add a separate click tracker or tracking redirect. Add a platform-specific sub-ID only if the affiliate program's official documentation confirms that parameter is supported and it will not alter the destination.
- Do not use emojis or pasted graphics. The MLGS editor warns against them.
- Prefer composing a fresh message. Do not load a saved email based only on its displayed name. If using a saved draft, verify the complete subject, body, destination, and preview before sending.
- Keep the currently selected sender and Perfect Timing setting unless there is a clear reason to change them.

## Lead selection and rotation

- Use **Mail by date**. The account review showed date-based groups of about 100 leads; the partner groups are not interest tags.
- For a first campaign, use the newest 9,000 leads by date. Choose 12,000 only when previous reported conversions and the offer's relevance support scaling.
- For subsequent campaigns, consult the private campaign log in the current conversation and exclude every date batch already mailed. Select the newest non-overlapping unmailed batches that total exactly 9,000 or 12,000. Do not send to the same “newest” cohort every day: with 100 new leads per day, daily 9,000-lead selections would overlap by about 8,900 recipients.
- If the interface cannot produce the exact target count, if date history is unclear, or if there is no non-overlapping cohort, stop rather than guessing or repeating recipients. Report the visible count and ask how Costas wants to proceed.
- Before submitting, verify the platform's selected-lead counter equals the chosen target exactly.

## Pre-send checks and submission

Before clicking **Send Email**:

1. Confirm the page is still the authenticated MLGS mailing form.
2. Confirm the subject accurately describes the message.
3. Open the MLGS preview. Confirm the chosen anchor words are visible, the raw URL is not exposed in the email body, and the link destination matches the supplied affiliate URL.
4. Confirm the final message includes the affiliate disclosure and the MLGS-generated compliance footer, including its opt-out method and required sender details. If the preview does not show a working unsubscribe option or required sender information, stop and ask Costas to resolve it.
5. Confirm the lead counter is exactly 9,000 or 12,000 and that the selected date batches do not overlap the private campaign history.

After those checks, submit exactly one mailing. Verify the success state and capture the campaign's visible identifier/count where available. Never submit twice because a page is slow; inspect the resulting page first.

## Records and privacy

- Record one aggregate campaign row in the current ChatGPT conversation using the columns in `docs/campaign-log.template.csv`. Record date range/cohort, offer name/domain, subject, anchor text, selected and sent counts, MLGS opens/clicks, conversions, and commission when reported. Mark unavailable results as pending; never estimate or invent them.
- Ask Costas to report conversion date, source tag/campaign, conversion type, and commission amount. Do not record a lead's name, email address, IP address, or other personal data.
- This GitHub repository is public. Never commit actual affiliate links, campaign copy, recipient data, browser credentials/cookies, or campaign performance rows. Keep the working ledger private; `campaign-log.csv` is ignored by Git.

## Scope

This is an on-demand, browser-assisted workflow. Do not create a recurring mailing schedule or claim that a GitHub-hosted runner can attach to Costas's local Chrome session.