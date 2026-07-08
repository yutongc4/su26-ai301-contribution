# Open Source Contribution Log Second selected session

## Contributor Information

* **Name:** [Yutong Chen]
* **GitHub Username:** [yutongc4]
* **Program:** CodePath AI301
* **Project:** Gramps Web
* **Project Repository:** https://github.com/gramps-project/gramps-web
* **Status:** Phase I Complete

---

# Phase I: Issue Selection

## Selected Issue

**Issue #507: Feature request: Provide the ability in Grampsweb to change the genealogical symbols**

https://github.com/gramps-project/gramps-web/issues/507

## Problem Summary

Gramps Web currently uses fixed genealogical symbols, such as the symbol displayed for a death date, and users do not have a way to change them. This can be a problem because genealogical symbols may have different cultural, religious, or personal meanings, so one fixed set is not appropriate for every user.

The issue asks for a way to customize these symbols, preferably through the Gramps Web user interface. Based on the maintainer’s guidance, the first implementation can focus on a per-user setting while preserving the current symbols as the default behavior.

## Why I Chose This Issue

I chose this issue because it is a clearly defined, user-facing improvement with guidance from an active maintainer. The issue is labeled `good first issue`, is currently unassigned, and does not have an existing pull request.

I am interested in this issue because it will allow me to:

1. Learn how Gramps Web stores and updates user preferences.
2. Gain experience working with JavaScript, Lit web components, and an existing settings interface.
3. Practice tracing hard-coded UI values throughout a larger codebase.
4. Improve accessibility and cultural flexibility for Gramps Web users.

The maintainer has identified a possible starting point: store the selected option with `this.appState.updateSettings`, similar to the language or home-person settings, and add a selector to `GrampsViewSettings.js`. The maintainer also confirmed that beginning with a per-user setting is an acceptable first scope.

## What “Fixed” Looks Like

The issue will be considered addressed when a user can choose an alternative genealogical symbol configuration in Gramps Web’s user settings.

For the initial implementation:

* The setting is stored per user.
* The current symbol behavior remains the default.
* A control is added to the user settings interface.
* Relevant hard-coded genealogical symbols use the selected configuration.
* Existing users who do not change the setting see no behavioral change.

## Initial Scope

For the first version, I plan to focus only on the per-user configuration suggested by the maintainer.

Possible future improvements, such as per-tree settings or a priority order of default, per-tree, and per-user values, are outside my initial scope unless the maintainer requests them.

I will also review how Gramps Desktop handles genealogical symbols to determine whether Gramps Web should initially provide predefined symbol sets or eventually allow users to customize individual symbols.

## Issue Selection Checklist

| Check                              | Result | Notes                                                                                               |
| ---------------------------------- | ------ | --------------------------------------------------------------------------------------------------- |
| I understand the problem           | ✅      | Genealogical symbols are currently fixed and cannot be customized.                                  |
| Scope fits the contribution period | ✅      | The maintainer approved starting with a smaller per-user implementation.                            |
| Matches skills or learnable skills | ✅      | The work involves frontend JavaScript, settings state, and UI components.                           |
| Issue is active and claimable      | ✅      | The issue is open, unassigned, and has recent maintainer guidance.                                  |
| Helpful context is available       | ✅      | The maintainer identified the state-management method and likely settings file.                     |
| Project has setup documentation    | ✅      | The repository includes a README, contributing guide, developer documentation, and a dev container. |

**Checklist score: 6/6**

## Maintainer Communication

I commented on the issue to express my interest and asked whether alternative symbol sets already existed and whether the first implementation should include per-tree settings.

The maintainer confirmed that:

* Alternative symbol sets are not currently defined.
* I can begin with a per-user setting.
* It is worth reviewing how Gramps Desktop handles symbol customization.

## Repository Fork

I forked the Gramps Web frontend repository:

https://github.com/[YOUR-GITHUB-USERNAME]/gramps-web

## Phase I Completion Checklist

* [x] Selected a live GitHub issue
* [x] Read the issue description and maintainer comments
* [x] Confirmed that the issue is open and unassigned
* [x] Commented on the issue
* [x] Summarized the problem and expected outcome
* [x] Explained why I selected the issue
* [x] Forked the correct project repository
* [x] Updated this contribution README
* [x] Marked Phase I Complete
