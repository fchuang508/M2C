# M2C — Motion to Contract
From Conversation to Inevitable Execution · by iMeeting

This repository holds two kinds of public project pages: **quotations** (报价单) and **co-creation covenants / contracts** (共创契约). Its long-term role is the M2C contract module for iMeeting, mounted under `https://imeeting.club/contracts/`.

The root domains `https://imeeting.club` and `https://www.imeeting.club` belong to the future iMeeting homepage repository, not this M2C repository. Contracts use neutral canonical URLs under `/contracts/{contractId}/`. Numbered project folders remain available as source/project archives and transition paths.

## Quotation page rules

- Each project folder should use `index.html` as the stable public URL for the latest official quotation.
- Versioned quotation files should keep their original filenames, such as `quotation-v3-20260529.html`.
- Version labels shown in the page footbar should use `Q-YYYYMMDD-vN`, where `YYYYMMDD` is the quotation date and `vN` is the quotation version.
- When a published file has a legacy filename, keep the file in place and mark it as a legacy archive in the footbar instead of renaming it.
- When a new quotation version becomes official, copy that full version into `index.html` and keep the versioned file as an archive.
- The latest `index.html` and every versioned quotation page should include the same fixed bottom version footbar.
- The footbar should identify the shared project, show whether the current page is latest or historical, link back to `index.html`, and open the version history list from the bottom.
- Existing quotation filenames should not be renamed after they have been published, so old public links continue to work.

## Covenant / contract page rules

- A covenant project is a resolution turned into a signed agreement among co-creators (共创人), not a buyer–seller quotation.
- Each canonical covenant folder uses `contracts/{contractId}/index.html` as the covenant body, and stores its source records (meeting minutes, speech log) alongside it, prefixed by the meeting number, e.g. `308247877-minutes.md`.
- A covenant should cite the resolution it is based on: organization, meeting number, date, validity, and vote result.
- Amounts or terms still under revision should be marked as provisional (暂定 · 以会后最终修正为准) rather than hard-locked.
- Versioned covenant files should use `contract-vN-YYYYMMDD.html` or another stable published filename, while the page label shown to readers should use `C-YYYYMMDD-vN`.
- When a covenant receives a later supplement, keep `index.html` as the latest public URL, preserve the earlier covenant as a version archive, and add a readable difference page when the supplement changes the contract body.

## Cloudflare Pages

- Project name: `m2c-contracts`
- Future canonical mount: `https://imeeting.club/contracts/`
- Temporary direct domain can be a Pages-provided domain or a subdomain such as `contracts.imeeting.club`.
- Output directory: repository root
- Build command: none
- Deploy command: `npm run deploy:cloudflare`
- Root domains and `www` redirects should be configured in the separate iMeeting homepage repository.

## Projects

- `01-semi-wallet-integration/` — Semi Wallet Integration · 报价单
- `02-imeeting-onboarding-video/` — iMeeting Onboarding 视频 · 报价单
- `contracts/` — M2C public contract index
- `contracts/c_20260627_coart-create-promotion/` — Co-Art Create Promotion · 艺术共创营系列宣传框架 · 共创契约（会议 308247877）
- `03-coart-create-promotion/` — legacy project folder for the same covenant
