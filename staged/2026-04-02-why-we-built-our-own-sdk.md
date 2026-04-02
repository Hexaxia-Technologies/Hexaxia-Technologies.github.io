# Why We Built Our Own SDK (And Why Your Platform Probably Needs One Too)

*How we turned our operations platform into a command-line powerhouse and eliminated hours of daily busywork.*

*April 2, 2026 | Hexaxia Technologies*

---

We run an IT services practice. Like most teams in our industry, we live inside our primary operations platform all day: logging tickets, tracking assets, managing invoices, monitoring alerts, writing internal documentation. The platform does what it's supposed to do.

But we kept running into the same friction: repetitive tasks that required clicking through the same screens, filling in the same forms, pulling the same reports. The kind of work that makes you think "there has to be a faster way to do this."

There was. The platform has a REST API. A good one. Well-documented, hundreds of endpoints, covering the full breadth of what the platform does.

What it didn't have was any tooling around that API. No SDK. No CLI. No way to say "show me all open tickets for this customer" from a terminal. No way for our automation systems to create an estimate, add line items, and log time without a human clicking through the UI.

## The Gap Nobody Filled

We checked. The third-party ecosystem was a handful of abandoned scripts and one wrapper library with zero adoption. The platform vendor hadn't released an official SDK. Nobody had built a CLI.

For a platform used by thousands of organizations, that's a surprising gap. Every one of those teams has people doing the same repetitive API-eligible work through a browser.

## What We Needed

Our requirements were straightforward:

- **A command-line interface** for daily operations. List open tickets. Search customers. Check compliance status on an asset. Send an invoice. All from the terminal, without opening a browser tab.

- **A typed client library** that our AI agents and automation scripts could import. We're building intelligent systems that manage operations, and they need programmatic access to the same data our team uses.

- **Output flexibility.** Tables for humans. JSON for scripts. Plain text for pipelines. One tool that serves all three audiences.

- **Security by default.** This tool touches customer data, invoices, and internal documentation. Credentials need to be stored properly, transmitted safely, and never leaked in logs or error messages.

## What It Changed

The impact was immediate.

A ticket that used to mean opening the browser, navigating to the customer, filling in the form, and adding a comment? Now it's one command. A compliance check across a customer's assets that used to take 15 minutes of clicking through individual records? Now it's a loop.

Our AI systems can now create estimates with line items, log billable time against tickets, and pull customer data without any human in the loop. That's not theoretical. We built out a real client proposal through the SDK on the first day we had it working.

The daily standup check that used to mean opening three different screens (open tickets, active alerts, unpaid invoices) is now three commands that run in two seconds.

## Security Wasn't an Afterthought

This tool touches customer records, financial data, asset inventories, and internal documentation. That's not a place where you bolt security on later.

From the first day, credentials are stored with restricted file permissions and never appear in URLs, logs, or error output. We ran a full security review against the codebase, the entire git history, and every dependency before we used it against live data. Input validation prevents the kind of subtle attacks that slip through when you're trusting user-supplied configuration values.

When you're building automation that operates on client data, security isn't a feature. It's the foundation.

## The Bigger Picture

Every platform with a REST API and no SDK is leaving value on the table. Both for their users and for themselves. The API exists. The documentation exists. But without tooling, only the most motivated developers will use it. Everyone else stays in the browser, doing manually what could be automated.

We built this for ourselves because we needed it. What happens next is something we're actively evaluating. It could stay internal, go open source, or become something bigger. The interest from other teams facing the same gap will probably decide that.

What we know is this: the gap between "has an API" and "has usable developer tooling" is where a lot of operational efficiency is hiding. If your platform has an API you're not using programmatically, you're probably leaving hours on the table every week.

If that sounds familiar, we'd like to hear about it. We're always looking for the next piece of complexity to remove.

**[Talk to us](https://hexaxia.tech/contact)**

---

*Hexaxia Technologies removes complexity from IT operations. We build AI-powered automation that helps businesses work smarter with the tools they already have.*
