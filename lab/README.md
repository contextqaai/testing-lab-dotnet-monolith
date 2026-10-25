# ContextQA lab — ASP.NET Core · monolith

Educational source fork of [NimblePros/eShopOnWeb](https://github.com/NimblePros/eShopOnWeb). Original history, notices and license are retained. This is not an endorsed integration or a customer production app.

**Status: source and exercises available. Public deployment, platform import and ContextQA run results are not verified.**

Starting source commit: `f21d6233b851897371c25c5e7ffa67bb8552dba8`.

## Setup and scope

Follow the maintained upstream setup. This is an ASP.NET Core monolith, not classic .NET Framework or Web Forms. Use the exact SDK/database configuration in this source and synthetic catalog data.

Follow the [original setup instructions](../README.md#upstream-project-documentation). See [stack/platform guidance](https://github.com/contextqaai/testing-lab/blob/main/PLATFORMS.md) for deployment boundaries.

## Exercises

| Scenario | Explicit assertion |
|---|---|
| Catalog | A seeded item can be located in the catalog. |
| Basket edit | Updating an item changes the quantity shown. |
| Calculation | Displayed totals match the fixture values. |
| Sign in | A configured test user reaches the signed-in view. |
| Navigation | The basket state remains consistent through the supported page navigation. |

These are acceptance exercises, not claims that upstream currently satisfies each desired requirement. Inspect the implemented workflow and fixtures before generating executable steps. Missing validation/auth may deliberately demonstrate a failure and must be disclosed.

## End-to-end lesson

Start an owned/authorized copy with synthetic fixtures. State the assertion, create/review a test in your authenticated ContextQA workspace, execute, and inspect the actual verdict. Introduce one disclosed regression in a separate variant, rerun the same assertion, fix the app and rerun. Confirm mutations against disposable data. Keep credentials and private reports out of this repository.

Record app commit/build, fixture/scenario version, browser/runner version, environment and timestamp with every real report. A cached report is recorded evidence, not a new run. No ContextQA report has been generated for this fork yet.

[ContextQA setup](https://contextqa.com/tutorials/getting-started-with-contextqa-test-automation/) · [Central catalog](https://github.com/contextqaai/testing-lab)
