# Friction Log

This document records the points where I became stuck while building the Tressa Health Shopify theme.

The purpose is to distinguish between gaps in syntax, architecture, platform knowledge and tooling so I can identify what needs more practice.

---

## Entry Template

**Date:**
**Task:**
**Expected:**
**Observed:**
**Friction type:** Syntax / Architecture / Platform knowledge / Tooling
**Initial hypothesis:**
**Documentation consulted:**
**Attempt:**
**Result:**
**What I learned:**

---

## 2026-08-04 — Setting Up Skeleton

**Task:** Add the Skeleton theme to the GitHub repo I had already created.

**Expected:** I thought I could run `shopify theme init` inside the repo and it would add the files there.

**Observed:** The command creates a new folder, so I would have ended up with one project folder inside another.

**Friction type:** Tooling / Platform knowledge

**Initial hypothesis:** I could initialize Skeleton somewhere else and then copy the files into my repo without copying its Git history.

**Attempt:** I created a temporary Skeleton project and copied the files into my existing repo while excluding the `.git` folder.

**Result:** It worked. My existing GitHub remote stayed connected.

**What I learned:** Before using an initialization command, check whether it modifies the current folder or creates a new one.

