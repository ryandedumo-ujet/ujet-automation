# ujet-automation

Central repo for UJET QA automation tools. Each tool lives in its own sub-repo and is linked here as a git submodule.

## Clone

```bash
git clone --recurse-submodules https://github.com/ryandedumo-ujet/ujet-automation.git
```

If you already cloned without submodules:

```bash
git submodule update --init --recursive
```

---

## Tools

### feature_flag
Manages feature flags across UJET staging environments. Supports restoring all flags to defaults or updating a single flag on a specified tenant. Credentials are pulled from 1Password automatically.

→ See [`feature_flag/feature-flag-agent.md`](feature_flag/feature-flag-agent.md) for usage

---

### regression_workflow
Analyzes PRs from a Jira filter or a single PR URL, runs the regression risk map script, then applies a reasoning layer to validate which test scenarios are genuinely in scope — and produces an actionable test plan with BrowserStack TCs.

→ See [`regression_workflow/regression-agent.md`](regression_workflow/regression-agent.md) for usage

---

### testcase-automation
Converts a Notion test plan (exported as Markdown) into a BrowserStack-compatible CSV ready for direct import into a test management project.

→ See [`testcase-automation/testcase-generation-process.md`](testcase-automation/testcase-generation-process.md) for usage
