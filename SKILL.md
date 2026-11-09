---
name: rs-legal-mcp-skill
description: Official Serbia (RS) legislation, multi-tier court precedent research, and citation verification skill.
version: 2.0.0
author: JurisAtlas
license: MIT
---

# Serbia Legal Research & Multi-Tier Case Law Skill (`rs-legal-mcp`)

Use this skill whenever the user asks a legal question, drafts a pleading or contract, or researches case law across any judicial instance in **Serbia (RS)**.

## Verification & Research Rules

1. **Citation Verification:** Never fabricate a statutory provision or case citation. Query `search_legislation`, `search_case_law`, `search_tiered_court_decisions`, or `verify_citation` before citing any authority (e.g., `Rev 1234/2023 or Službeni glasnik RS br. 12/2024`).
2. **Multi-Tier Judicial Coverage:**
   - **First Instance (Trial / Municipal / District):** Osnovni sudovi (66 Basic Courts), Viši sudovi (25 Higher Courts in first-instance jurisdiction), Privredni sudovi (16 Commercial Courts) & Prekršajni sudovi
   - **Second Instance (Cantonal / Regional / Appellate):** 4 Apelaciona suda (Beograd, Novi Sad, Niš, Kragujevac), Viši sudovi (appellate jurisdiction), Privredni apelacioni sud & Upravni sud Republike Srbije
   - **Supreme & Constitutional Instance:** Vrhovni sud Republike Srbije (vrhovni.sud.rs) & Ustavni sud Republike Srbije (ustavni.sud.rs)
   - **Primary Tiered Database:** Pravno-informacioni sistem RS - Baza sudske prakse (pravno-informacioni-sistem.rs) & Portali Apelacionih Sudova (`https://www.pravno-informacioni-sistem.rs/SlGlasnikPortal/sudska-praksa`)
