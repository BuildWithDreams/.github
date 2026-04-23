# BuildWithDreams

**Autonomous Infrastructure. Idempotent Workflows. Agent-Driven Development.**

---

We explore the intersection of the [Verus DREAM framework](https://verus.io) and autonomous AI agents. Every piece of infrastructure we build is:

- **Self-documenting** — code and documentation live together, updated in the same commit
- **Repeatable** — any VPS can be provisioned from scratch using our Ansible playbooks
- **Agent-native** — built to be operated by Hermes-series LLMs, not just humans

## The Ecosystem

| Repository | Purpose |
|------------|---------|
| [`dream-pbaas-provisioning`](https://github.com/BuildWithDreams/dream-pbaas-provisioning) | Ansible playbooks for idempotent VPS provisioning |
| [`docker-verusd`](https://github.com/BuildWithDreams/docker-verusd) | Dockerized Verus Protocol blockchain nodes |
| [`dream-info`](https://github.com/BuildWithDreams/dream-info) | DREAM framework — Decentralized, Rights-preserving, Encrypted Application Model |
| [`dream-session-digest`](https://github.com/BuildWithDreams/dream-session-digest) | Nightly session digest — Venice summaries, GitHub evidence, email + Jekyll blog |
| [`dream-blog`](https://buildwithdreams.github.io/dream-blog) | Daily session digests and work logs |

## How We Work

We practice what we preach. Commits are written by `dream-hermes-agent`, an autonomous LLM agent operating from a Hermes CLI session. Every workflow is codified — no one-off SSH commands, no manual steps that can't be reproduced.

Infrastructure changes flow through this loop:

```
Code change → Skill update → CI secrets scan → Code review → Merge
```

## Security

- No credentials in git — ever
- Pre-commit hooks + CI scan for private IPs and key paths on every push
- Secrets stored in `group_vars/production-local.yml`, excluded from version control

## License

All repositories are MIT licensed unless noted otherwise.

---

*This organization is operated by autonomous agents. Human oversight is maintained, but the day-to-day engineering is done by AI.*
