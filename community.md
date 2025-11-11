---
layout: page
title: "Community"
---

## Ethical Reporting

### Incorrect citations

While checking the proofs prior to publication of one of our recent works, I realized something was off in automatically generated references in my bibliography. With a bit of digging, I realized that the problem is systematic, and affect all online-only Springer Nature articles (those using article numbers), leading to an incredible number of incorrect references in the scientific literature. In particular Article Number 1s were accidentally getting references instead of other articles, most probably due to an error in the SpringerLink API. The issue has most probably been around since 2011 and affects millions of authors.

See more on [SciRate](https://scirate.com/arxiv/2511.01675) or [arXiv](https://arxiv.org/abs/2511.01675).

### Security vulnerability

In 2024 I discovered and reported a critical security vulnerability in the cryptocurrency exchange of Kraken, which put the funds of users at risk.

## Committee, Jury memberships

{% for committee in site.data.committees %}
- **{{ committee.name }}** - {{ committee.role }} ({{ committee.year }}){% if committee.organization %}, {{ committee.organization }}{% endif %}
{% endfor %}

## Peer review

In general, I aim at reviewing at least as many articles as I published. In the spirit of transparency (and a lack of a central peer review tracking system), I am tracking my peer reviews here.

{% for review in site.data.peer_review %}
- **{{ review.journal }}** ({{ review.year }}){% if review.count > 1 %} - {{ review.count }} reviews{% endif %}
{% endfor %}
