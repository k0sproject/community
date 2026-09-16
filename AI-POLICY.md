# AI Policy

This document outlines the guidelines and principles for the use of artificial intelligence (AI) within our organization.

We use the [Kubernetes AI policy](https://www.kubernetes.dev/docs/guide/pull-requests/#ai-guidance) as the base for our own AI policy.

These policies reflects our approach to AI: embrace it as a tool, and tool only, never let AI to replace human judgement, understanding, common sense, and critical thinking.

**TL;DR;** AI can be used as a tool to assist in development, but humans must remain accountable, engaged, and in control of all contributions.

## Coverage

This policy applies to all contributors, maintainers, and reviewers involved in the development and maintenance of our projects. It covers the use of AI tools in code contributions, documentation, issue tracking, and any other project-related activities.

By default this covers all k0project repositories, unless a sub-repository has its own deviations explicitly stated.

## Human accountability

While we all probably use AI tools in our daily work, it is essential to remember that humans remain ultimately accountable for the contributions. Since all the CNCF projects require DCO/CLA sign-offs, one CANNOT make AI as accountable party.

This policy prohibits:

- Listing AI as a co-author on commits
- Using AI co-signing on commits
- Adding trailers like "assisted-by" or "co-developed" that attribute work to AI

## Human engagement required

Project maintainers, reviewer and other contributors are expecting to engage directly with humans. This means that one cannot rely on AI tools to respond to review or issue comments. If you cannot personally respond and engage, without using AI tools, in the discussion to explain your proposed changes (whether or not AI assisted in generating them), your contribution will be rejected. This ensures that design decisions are properly communicated and understood and also we leave a written trail of crumbs for future reference.

When contributing, you must verify any AI-generated changes through self-review, testing and personal understanding BEFORE submitting them. It's not really enough for the code to work, you must understand how and why it works and be ready to explain your approach to maintainers and reviewers.
