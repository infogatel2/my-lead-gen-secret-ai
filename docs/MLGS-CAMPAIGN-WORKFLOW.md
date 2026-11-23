# Campaign Run Sequence

This playbook is designed for one user-triggered campaign at a time. The user supplies the affiliate link; the assistant confirms the live MLGS browser session, researches the offer, writes and formats the message, selects a verified cohort, sends once, and records aggregate results.

## 1. Confirm the session

Check the existing Chrome tab for the MLGS member mailing page. Verify the member navigation and mailing controls are visible. If signed out or unavailable, stop and ask Costas to connect the page. Do not collect login credentials in chat.

## 2. Review the offer and link

- Identify the final merchant/product and review its official offer details.
- Keep the affiliate destination exactly as supplied. Do not add a link shortener or external click tracker.
- If an official sub-ID parameter is supported, use a unique campaign ID. Otherwise use MLGS campaign statistics and the private campaign ledger for attribution.
- Never test the affiliate link by completing a signup or purchase.

## 3. Create the email

Use a short, accurate subject and a conversational body that speaks to business-opportunity/internet-marketing readers without promising income. Make the opening intriguing but truthful. Include one CTA as a rich-text hyperlink on natural anchor copy, not a visible raw URL, and include an affiliate disclosure. Use no emojis or pasted graphics.

## 4. Select the cohort

Default to 9,000 for the first campaign. Use 12,000 only if prior reported conversions and the offer's relevance justify a larger send.

Use **Mail by date** and select date groups totaling exactly the chosen number. The reviewed account displayed around 100 leads per date. Consult prior campaign rows and skip dates already mailed. The newest cohort may be used first; later runs must use the newest available non-overlapping dates. If there is no suitable unmailed cohort or the selected count is not exact, stop without sending.

## 5. Preview, send, and record

Preview the email and verify the hidden link text, actual link destination, subject, affiliate disclosure, MLGS footer/unsubscribe details, and selected-lead count. Then send one campaign and verify the success state.

Record the campaign's date range, audience count, subject, anchor text, offer/domain, source tag if supported, MLGS open/click counts, and any reported conversions/commission. Keep the detailed ledger private because this repository is public.
