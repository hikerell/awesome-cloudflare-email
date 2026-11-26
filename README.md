# Awesome Cloudflare Email [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> Open-source projects, libraries and guides that turn Cloudflare Email Routing and Email Sending into inboxes, sending APIs, newsletters and agent mailboxes.

Cloudflare receives mail for your domain for free (Email Routing) and can send it from a Worker (Email Sending), but it gives you no inbox, API or user interface. The projects below fill that gap, almost all of them inside your own Cloudflare account.

Licenses are as stated in each repository. 💰 marks a paid product. Last checked: October 24, 2026.

## Contents

- [Official resources](#official-resources)
- [Webmail and team inboxes](#webmail-and-team-inboxes)
- [Sending APIs](#sending-apis)
- [Newsletters and broadcasts](#newsletters-and-broadcasts)
- [Inboxes for AI agents](#inboxes-for-ai-agents)
- [Help desk and shared inbox](#help-desk-and-shared-inbox)
- [Temporary and disposable email](#temporary-and-disposable-email)
- [Notifications and forwarding](#notifications-and-forwarding)
- [Libraries](#libraries)
- [Tools](#tools)
- [Guides and articles](#guides-and-articles)
- [Related lists](#related-lists)

## Official resources

- [Email Routing](https://developers.cloudflare.com/email-routing/) - Receive mail for your domain and forward it or hand it to a Worker. Free on every plan.
- [Email Workers](https://developers.cloudflare.com/email-routing/email-workers/) - Process incoming mail in a Worker's `email()` handler.
- [Email Workers runtime API](https://developers.cloudflare.com/email-routing/email-workers/runtime-api/) - `ForwardableEmailMessage`, `reply()`, `forward()` and `setReject()`.
- [Send emails from Workers](https://developers.cloudflare.com/email-routing/email-workers/send-email-workers/) - The `send_email` binding.
- [Email Service](https://developers.cloudflare.com/email-service/) - Email Sending and Email Routing documentation.
- [Email Service pricing](https://developers.cloudflare.com/email-service/platform/pricing/) - Sending needs Workers Paid: 3,000 emails a month included, then $0.35 per 1,000. Receiving is unlimited.
- [Email Service limits](https://developers.cloudflare.com/email-service/platform/limits/) - Message size, recipients and rate limits.

## Webmail and team inboxes

A browser inbox for the addresses on your domains.

- [cloud-mail](https://github.com/maillab/cloud-mail) - All-in-one mailbox service with multiple users and roles. `MIT`
- [Mailflare](https://github.com/hieunc229/mailflare) - Email for teams, with users, permissions and multiple domains; sends through Cloudflare, Resend or Amazon SES. `AGPL-3.0`
- [agentic-inbox](https://github.com/cloudflare/agentic-inbox) - Cloudflare's self-hosted email client with a built-in AI agent, behind Cloudflare Access. `Apache-2.0`
- [HQBase](https://github.com/HQBase/hqbase) - AI-native email workspace for teams, with shared mailboxes. `AGPL-3.0`
- [OmniMail](https://github.com/mibgb65-cloud/OmniMail) - Multi-domain webmail on Workers, D1, R2 and Queues, sending through Resend. `MIT`
- [Email Explorer](https://github.com/G4brym/email-explorer) - Serverless Worker for sending and receiving email. `MIT`
- [Cloud Mail Plus](https://github.com/AndrewYukon/cloud-mail-plus) - cloud-mail extended with Cloudflare Email Service sending and an external API. `MIT`
- [hpc-mail](https://github.com/riba2534/hpc-mail) - Multi-domain, multi-user mailbox with catch-all receiving, code extraction and a REST API. `MIT`
- [heyflare](https://github.com/doable-team/heyflare) - HEY-style client (Screener, Imbox, Feed) for custom domains plus Gmail and IMAP accounts. `MIT`
- [cloudflare-mail-server](https://github.com/chawuciren/cloudflare-mail-server) - Multi-user business email: Email Routing in, Resend out, on a Node.js and SQLite server rather than Workers.
- 💰 [MarkRelay](https://markrelay.com) - Team webmail, a scoped HTTP API, signed webhooks, broadcasts and agent mailboxes, installed into your own Cloudflare account. Commercial, closed source.

## Sending APIs

A Resend-style HTTP API for transactional email on your own Cloudflare account.

- [EmailFlare](https://github.com/0xdps/emailflare) - Sending platform on Cloudflare Email Sending with a REST API, admin UI, templates and domain management. `MIT`
- [MailySend](https://github.com/GagnDeep/mailysend) - Resend-compatible API with transactional sending, broadcasts, automations and inbound. `MIT`

## Newsletters and broadcasts

Lists, campaigns and unsubscribe handling on Workers and D1.

- [Kōlea](https://github.com/robconery/kolea) - Broadcasts, drip sequences and transactional email in one Cloudflare app. `MIT`
- [Ownlist](https://github.com/pfstr/ownlist) - Serverless newsletter on your own Cloudflare account (Workers and D1). `MIT`

Cloudflare's Email Service terms are written for transactional email; check them before sending bulk or marketing mail.

## Inboxes for AI agents

Mailboxes that an agent reads and answers over an API or MCP.

- [DearAgent](https://github.com/panda-sandeep/dearagent) - Email inbox API for AI agents with an MCP server; a self-hosted AgentMail alternative. `AGPL-3.0`
- [Goshen Email](https://github.com/boringcomputers/goshen-email) - Agent inboxes with per-mailbox API keys, a REST API, CLI, MCP server and a dashboard; also offered as a hosted service.
- [MailClaw](https://github.com/missuo/mailclaw) - Catch-all inbox with a token-protected API, full-text search and an agent skill.
- [smails](https://github.com/pexni/smails) - Disposable inboxes for agents on Durable Objects, with a CLI and MCP. `MIT`
- [ni-mail](https://github.com/mskatoni/ni-mail) - Minimal Worker that receives mail for your domain and exposes it over an HTTP API. `Apache-2.0`

## Help desk and shared inbox

Tickets, assignment and customer timelines for support teams.

- [saasmail](https://github.com/choyiny/saasmail) - Email for SaaS teams; members see the inboxes assigned to them; WebMCP support. `Apache-2.0`
- [ResolveHQ](https://github.com/mirza-rizvi/ResolveHQ) - Help desk on Workers, D1, R2 and Queues with a shared inbox, threading and AI assistance.

## Temporary and disposable email

Throwaway addresses for sign-ups and testing.

- [cloudflare_temp_email](https://github.com/dreamhunter2333/cloudflare_temp_email) - Temporary mail with attachments, sending, an IMAP/SMTP proxy and a Telegram bot. `MIT`
- [MoeMail](https://github.com/beilunyang/moemail) - Temporary mail built with Next.js on Cloudflare. `MIT`
- [vmail](https://github.com/oiov/vmail) - Temporary mail on a Worker and D1 with multiple domains and an open API. `GPL-3.0`
- [smail](https://github.com/akazwz/smail) - Temporary mail with a real-time inbox. `MIT`
- [temp-mail](https://github.com/vwh/temp-mail) - A Worker that acts as a temporary inbox. `MIT`
- [Tempik](https://github.com/hirotomasato/tempik) - Disposable email service running entirely on Workers. `MIT`
- [SpinupMail](https://github.com/ridvan/spinupmail) - Unlimited temporary addresses with attachments. `MIT`
- [FreeTempMail](https://github.com/PennyJoly/FreeTempMail) - Temporary mail service built on Nuxt and Cloudflare, with i18n. `MIT`
- [MailGate](https://github.com/Dicka18/mailgate) - Receive-only OTP and magic-link inbox on Workers, D1, Email Routing and Cron, with strict allowlist rejection, sandboxed HTML preview, RFC822 simulator, zero-dependency Playwright/E2E SDK (waitForOtp()), and an optional HMAC-signed webhook bridge. MIT

## Notifications and forwarding

- [mail2telegram](https://github.com/tbxark/mail2telegram) - Receive email in Telegram, with push notifications and a Mini App inbox. `MIT`
- [Auth Inbox](https://github.com/TooonyChen/AuthInbox) - Collects verification codes from incoming mail and shows them in one place. `MIT`

## Libraries

- [postal-mime](https://github.com/postalsys/postal-mime) - Email parser for browsers and serverless runtimes; the usual way to parse mail in an Email Worker.
- [MIMEText](https://github.com/muratgozel/MIMEText) - RFC 5322 message builder for JavaScript runtimes, often used with the `send_email` binding. `MIT`
- [worker-mailer](https://github.com/zou-yu/worker-mailer) - SMTP client for Workers, to send through an external SMTP server. `MIT`
- [Cloudflare Email Kit](https://github.com/JacobLinCool/cloudflare-email-kit) - Toolkit for incoming and outgoing mail in Workers. `MIT`
- [email-worker](https://github.com/webbertakken/email-worker) - Lightweight tool to process email directly in Cloudflare. `MIT`

## Tools

- [dmarc-email-worker](https://github.com/cloudflare/dmarc-email-worker) - Cloudflare's processor for DMARC aggregate reports received through Email Workers. `MIT`

## Guides and articles

- [Cloudflare is now the cheapest email provider at $354/mo](https://levels.io/cloudflare-cheapest-email-provider) - What a million emails a month cost on Cloudflare compared with other providers.
- [Cloudflare Email Sending: pricing and setup](https://markrelay.com/docs/cloudflare-email-sending) - Onboarding a domain, sending from a Worker or over HTTP, and a cost calculator against Resend, SES and Postmark.
- [Free custom domain email with Cloudflare](https://markrelay.com/docs/free-custom-domain-email-cloudflare) - Receive with Email Routing, then three ways to send from the same address.
- [Reply from a Cloudflare Email Routing address](https://markrelay.com/docs/cloudflare-email-routing-reply) - Why replies come from your Gmail address and how to send from the routed address instead.

## Related lists

- [awesome-cloudflare](https://github.com/zhuima/awesome-cloudflare) - Cloudflare tools, open-source projects and guides in general.
- [awesome-selfhosted](https://github.com/awesome-selfhosted/awesome-selfhosted#communication---email---complete-solutions) - Self-hosted email servers and clients beyond Cloudflare.

## Contributing

Know a project that belongs here? See [CONTRIBUTING.md](CONTRIBUTING.md). Projects should run on or be built for Cloudflare Email Routing or Email Sending and have been updated in the last twelve months.

Maintained by [@hikerell](https://github.com/hikerell), who also builds MarkRelay (listed above).
