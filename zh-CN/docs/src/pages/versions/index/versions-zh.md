# Material-UI 版本号

<p class="description">You can come back to this page and switch the version of the docs you're reading at any time.</p>

## 稳定版本

The most recent version is recommended in production.

{{"demo": "pages/versions/StableVersions.js", "hideHeader": true}}

## 最新版本

Here you can find the latest unreleased documentation and code. You can use it to see what changes are coming and provide better feedback to Material-UI contributors.

{{"demo": "pages/versions/LatestVersion.js", "hideHeader": true}}

## Versioning strategy

We recognize that you need **stability** from the Material-UI library. Stability ensures that reusable components and libraries, tutorials, tools, and learned practices don't become obsolete unexpectedly. Stability is essential for the ecosystem around Material-UI to thrive.

This document contains **the practices that we follow** to provide you with a leading-edge UI library, balanced with stability. We strive to ensure that future changes are always introduced in a predictable way. We want everyone who depends on Material-UI to know when and how new features are added, and to be well-prepared when obsolete ones are removed.

Material-UI 严格遵循 [Semantic Versioning 2.0.0](https://semver.org/) 语义化版本规范。 Material-UI 的版本号由三部分组成：`主版本号.次版本号.修订版本号`。 版本号的选择是根据更新内容的数量决定

- **Major releases** contain significant new features, some but minimal developer assistance is expected during the update. When updating to a new major release, you may need to run update scripts, refactor code, run additional tests, and learn new APIs.
- **Minor releases** contain important new features. Minor releases are fully backward-compatible; no developer assistance is expected during update, but you can optionally modify your apps and libraries to begin using new APIs, features, and capabilities that were added in the release.
- **Patch releases** are low risk, contain bug fixes and small new features. No developer assistance is expected during update.

## 发布周期

We work toward a regular schedule of releases, so that you can plan and coordinate your updates with the continuing evolution of Material-UI.

通常情况下, 你可以根据以下的发布周期来预测:

- 每六个月发布一个**主版本**
- 1-3 **minor** releases for each major release.
- A **patch** release every week (anytime for urgent bugfix).

## 发布计划

> 免责声明: 日期作为一般指导提供, 我们可以在必要时调整, 以确保交付高质量的代码。

| 日期      | 版本                         |
|:------- |:-------------------------- |
| 2019年1月 | `@material-ui/core` v4.0.0 |
| 2019年7月 | `@material-ui/core` v5.0.0 |

你可以在 [ 我们的里程碑 ](https://github.com/mui-org/material-ui/milestones) 中查看更详细的概述。

## Support policy

We only support the latest version of Material-UI. We don't yet have the resources to offer [LTS](https://en.wikipedia.org/wiki/Long-term_support) releases.

## Deprecation practices

Sometimes **"breaking changes"**, such as the removal of support for select APIs and features, are necessary.

To make these transitions as easy as possible, we make two commitments to you:

- We work hard to minimize the number of breaking changes and to provide migration tools when possible.
- We follow the deprecation policy described here, so you have time to update your apps to the latest APIs and best practices.

To help ensure that you have sufficient time and a clear path to update, this is our deprecation policy:

- 我们会在更新日志中公布过时的功能, 并在可能的情况下, 在运行时发出警告。
- 当我们公布一个过时的功能时, 同时会提供一个最佳的更新方法。
- We support existing use of a stable API during the deprecation period, so your code will keep working during that period.
- We only make peer dependency updates (React) that require changes to your apps in a major release.