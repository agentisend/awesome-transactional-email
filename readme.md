# Awesome Transactional Email [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> Email an application sends to one person because of something that person did: receipts, password resets, sign-in codes, alerts.

APIs, relays, servers, testing tools, deliverability checks, template tools, libraries and MCP servers for sending it.

This list is maintained by AgentiSend, which is listed under Email APIs. Every other entry is described from its own website or repository. Corrections are welcome: see [contributing](contributing.md).

## Contents

- [Email APIs](#email-apis)
- [SMTP Relays](#smtp-relays)
- [Open-Source Mail Transfer Agents](#open-source-mail-transfer-agents)
- [Self-Hosted Sending Platforms](#self-hosted-sending-platforms)
- [Testing and Development](#testing-and-development)
- [Deliverability and DNS](#deliverability-and-dns)
- [Templates](#templates)
- [Libraries](#libraries)
- [MCP Servers](#mcp-servers)
- [AI Agent Guardrails](#ai-agent-guardrails)
- [Standards and Sender Requirements](#standards-and-sender-requirements)
- [Pricing Data](#pricing-data)

## Email APIs

- [AgentiSend](https://agentisend.com) - Transactional email API for applications and AI agents, with per-key send budgets and a kill switch. Maintained by the authors of this list.
- [Amazon SES](https://aws.amazon.com/ses/) - AWS email service billed per 1,000 emails, with an SMTP interface and an HTTPS API.
- [Bird Email API](https://bird.com/email-api) - Email API from Bird, which acquired SparkPost.
- [Brevo](https://www.brevo.com/products/transactional-email/) - Marketing platform with a transactional email API and SMTP relay.
- [Cloudflare Email Service](https://developers.cloudflare.com/email-service/) - Sending and routing email from Cloudflare Workers.
- [Elastic Email](https://elasticemail.com) - Email API and marketing platform.
- [Loops](https://loops.so) - Email platform for SaaS with marketing and transactional sending, priced by contacts.
- [Mailgun](https://www.mailgun.com) - Email API and SMTP service with inbound routing and email validation.
- [MailerSend](https://www.mailersend.com) - Transactional email API and SMTP with a template builder and inbound routing.
- [Mailjet](https://www.mailjet.com) - Email API and SMTP relay with a marketing editor.
- [Mailtrap](https://mailtrap.io) - Email API and SMTP for sending, alongside a testing sandbox.
- [Postmark](https://postmarkapp.com) - Transactional email API and SMTP that separates transactional and broadcast streams.
- [Resend](https://resend.com) - Email API from the team behind React Email, with SMTP and inbound email.
- [SendGrid](https://www.twilio.com/en-us/sendgrid/email-api) - Twilio's email API and SMTP relay.

## SMTP Relays

- [Amazon SES SMTP interface](https://docs.aws.amazon.com/ses/latest/dg/send-email-smtp.html) - SES credentials for any client that speaks SMTP.
- [SMTP2GO](https://www.smtp2go.com) - SMTP relay and email API with a free plan of 1,000 emails a month.

## Open-Source Mail Transfer Agents

- [Exim](https://www.exim.org) - Mail transfer agent for Unix-like systems, configured in a single run-time file.
- [Haraka](https://github.com/haraka/Haraka) - Event-driven SMTP server in Node.js, extended with plugins.
- [KumoMTA](https://github.com/KumoCorp/kumomta) - High-volume outbound MTA written in Rust and configured in Lua.
- [Maddy](https://github.com/foxcpp/maddy) - Composable all-in-one mail server in Go.
- [Mox](https://github.com/mjl-/mox) - Full-featured mail server in Go for low-maintenance self-hosted email.
- [OpenSMTPD](https://www.opensmtpd.org) - SMTP server from the OpenBSD project.
- [Postfix](https://www.postfix.org) - Widely deployed MTA with a security-focused design.
- [Stalwart](https://github.com/stalwartlabs/stalwart) - Mail and collaboration server in Rust (SMTP, IMAP, JMAP).
- [ZoneMTA](https://github.com/zone-eu/zone-mta) - Outbound MTA in Node.js with sending zones and plugins.

## Self-Hosted Sending Platforms

- [Plunk](https://github.com/useplunk/plunk) - Open-source email platform for transactional and marketing email, also sold as a hosted service.
- [Postal](https://github.com/postalserver/postal) - Mail delivery platform for incoming and outgoing email with an HTTP API.
- [Scribase Mail](https://github.com/caelum0x/scribase-mail-studio) - AGPL-3.0 email platform with a Resend-compatible API, SMTP relay, campaigns and webhooks, self-hostable or hosted.

## Testing and Development

- [Ethereal](https://ethereal.email) - Fake SMTP service that catches mail and never delivers it.
- [Inbucket](https://github.com/inbucket/inbucket) - Disposable webmail server with SMTP, POP3 and a REST API.
- [MailDev](https://github.com/maildev/maildev) - SMTP server with a web interface for viewing mail during development.
- [Mailosaur](https://mailosaur.com) - Hosted inboxes and SMS numbers for automated email tests.
- [Mailpit](https://github.com/axllent/mailpit) - SMTP testing server with a web UI and an API, inspired by MailHog.
- [Mailtrap Email Sandbox](https://mailtrap.io/email-sandbox/) - Hosted inbox that captures staging and test mail.
- [smtp4dev](https://github.com/rnwood/smtp4dev) - Fake SMTP server for development and testing, with a web UI.

## Deliverability and DNS

- [checkdmarc](https://github.com/domainaware/checkdmarc) - Python parser and validator for SPF and DMARC records.
- [DKIM Validator](https://dkimvalidator.com) - Send a message to a test address and get the DKIM, SPF and SpamAssassin result.
- [Google Postmaster Tools](https://postmaster.google.com) - Gmail's spam rate, authentication and delivery error reports for your domain.
- [Internet.nl email test](https://internet.nl/test-mail/) - Checks a domain's SPF, DKIM, DMARC, STARTTLS and DANE.
- [Learn DMARC](https://www.learndmarc.com) - Interactive walkthrough that shows SPF, DKIM and DMARC evaluating a message you send.
- [mail-tester](https://www.mail-tester.com) - Spam score for one test message.
- [Microsoft SNDS](https://sendersupport.olc.protection.outlook.com/snds/) - Outlook.com data on mail from IP addresses you control.
- [MxToolbox](https://mxtoolbox.com) - DNS, MX, SPF, DKIM and DMARC lookups.
- [parsedmarc](https://github.com/domainaware/parsedmarc) - Python package and CLI that parses DMARC aggregate and forensic reports.
- [Postmark DMARC Digests](https://dmarc.postmarkapp.com) - Free DMARC monitoring that sends a weekly digest of your reports.

## Templates

- [Can I email](https://www.caniemail.com) - Support tables for HTML and CSS features across email clients.
- [jsx-email](https://github.com/shellscape/jsx-email) - JSX components that render email HTML.
- [Maizzle](https://maizzle.com) - Email framework built on Tailwind CSS.
- [MJML](https://mjml.io) - Markup language that compiles to responsive email HTML.
- [React Email](https://github.com/resend/react-email) - React components and a preview server for building email.

## Libraries

- [Action Mailer](https://guides.rubyonrails.org/action_mailer_basics.html) - Mail in Ruby on Rails.
- [Django Anymail](https://github.com/anymail/django-anymail) - Django email backends and webhooks for most email APIs.
- [go-mail](https://github.com/wneessen/go-mail) - Mail library for Go.
- [Laravel Mail](https://laravel.com/docs/mail) - Mail in Laravel, with drivers for SMTP and several APIs.
- [lettre](https://github.com/lettre/lettre) - Mailer library for Rust.
- [Nodemailer](https://nodemailer.com) - Node.js email sending with pluggable transports.
- [PHPMailer](https://github.com/PHPMailer/PHPMailer) - Email sending library for PHP.
- [Symfony Mailer](https://symfony.com/doc/current/mailer.html) - Mail in Symfony, with transports for SMTP and several APIs.

## MCP Servers

- [AgentiSend MCP](https://agentisend.com/docs/guides/mcp) - Hosted MCP server for sending and reading mail with budgets per agent. Maintained by the authors of this list.
- [AgentMail MCP](https://github.com/agentmail-to/agentmail-mcp) - MCP server for AgentMail inboxes.
- [Mailgun MCP](https://github.com/mailgun/mailgun-mcp-server) - MCP server for the Mailgun API.
- [Postmark MCP](https://github.com/ActiveCampaign/postmark-mcp) - Postmark's MCP server for sending, templates and message search.
- [Resend MCP](https://github.com/resend/resend-mcp) - Resend's MCP server for sending email and working with the Resend API.

## AI Agent Guardrails

- [agent-email-guard](https://github.com/agentisend/agent-email-guard) - Send budgets, loop detection, kill switch and approval holds for agents that send email, with any provider. Maintained by the authors of this list.

## Standards and Sender Requirements

- [Gmail email sender guidelines](https://support.google.com/a/answer/81126) - Gmail's requirements for authentication, unsubscribe and spam rate.
- [RFC 7489](https://www.rfc-editor.org/rfc/rfc7489) - DMARC.
- [RFC 8058](https://www.rfc-editor.org/rfc/rfc8058) - One-click unsubscribe with `List-Unsubscribe-Post`.
- [Yahoo sender best practices](https://senders.yahooinc.com/best-practices/) - Yahoo's requirements for bulk and transactional senders.

## Pricing Data

- [email-api-pricing](https://github.com/agentisend/email-api-pricing) - Open dataset of published email API prices, each row with its source URL and date. Maintained by the authors of this list.
