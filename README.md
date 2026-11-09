# Serbia Legal Research MCP Server (`rs-legal-mcp`)

**[Srpski](#lang-sr) | [English Documentation](#english-documentation)**

---

<a id="lang-sr"></a>
## Pravni MCP Server (`rs-legal-mcp`) — Srpski

### O ovom repozitorijumu

Ovaj repozitorijum sadrži Model Context Protocol (MCP) server koji povezuje vašu AI aplikaciju (Claude Desktop, Cursor, Windsurf, VS Code / Copilot, Cline ili Antigravity) sa službenim glasnicima i bazama sudske prakse za **Serbia** (prvostepeni osnovni/opštinski i privredni sudovi, drugostepeni apelacioni/okružni/kantonalni i viši sudovi, kao i vrhovni i ustavni sudovi).

### Brza instalacija (Izbor AI aplikacije)

1. **Preuzimanje:** Kliknite na **`<> Code` -> `Download ZIP`** i raspakujte arhivu na računaru.
2. **Pokretanje:** Dvokliknite na **`Click_Here_To_Install_Windows.bat`** (Windows) ili **`Click_Here_To_Install_Mac.command`** (macOS).
3. **Izbor AI klijenta:** U instalacionom prozoru izaberite AI aplikacije koje koristite (Claude, Cursor, Windsurf, VS Code, Antigravity), kliknite na dugme za instalaciju i ponovo pokrenite izabranu AI aplikaciju.

**Bezbednosna napomena:** Program radi u izolovanom režimu čitanja (read-only) i ne pristupa niti menja vaše lične datoteke na računaru.

### Sudske instance i službeni izvori

| Sudska instanca | Obuhvaćeni sudovi |
|:---|:---|
| **1. Stepen (Prvostepeni sudovi)** | Osnovni sudovi (66 Basic Courts), Viši sudovi (25 Higher Courts in first-instance jurisdiction), Privredni sudovi (16 Commercial Courts) & Prekršajni sudovi |
| **2. Stepen (Apelacioni, okružni, kantonalni i viši sudovi)** | 4 Apelaciona suda (Beograd, Novi Sad, Niš, Kragujevac), Viši sudovi (appellate jurisdiction), Privredni apelacioni sud & Upravni sud Republike Srbije |
| **3. Stepen (Vrhovni i Ustavni sud)** | Vrhovni sud Republike Srbije (vrhovni.sud.rs) & Ustavni sud Republike Srbije (ustavni.sud.rs) |

- **Pravno-informacioni sistem Republike Srbije (pravno-informacioni-sistem.rs):** [https://www.pravno-informacioni-sistem.rs](https://www.pravno-informacioni-sistem.rs) (`pravno-informacioni-sistem.rs`, `parlament.gov.rs`, `paragraf.rs`)
- **Pravno-informacioni sistem RS - Baza sudske prakse (pravno-informacioni-sistem.rs) & Portali Apelacionih Sudova:** [https://www.pravno-informacioni-sistem.rs/SlGlasnikPortal/sudska-praksa](https://www.pravno-informacioni-sistem.rs/SlGlasnikPortal/sudska-praksa) (`vrh.sud.rs`, `vrhovni.sud.rs`, `sudskapraksa.sud.rs`, `ustavni.sud.rs`, `pravno-informacioni-sistem.rs`, `paragraf.rs`, `bg.ap.sud.rs`, `ns.ap.sud.rs`)

---

<a id="english-documentation"></a>
## English Documentation

Model Context Protocol (MCP) server providing live, read-only access to **Serbia (RS)** legislation, official gazettes, multi-tier judicial decisions (First Instance, Regional/Cantonal/Appellate, and Supreme/Constitutional courts, including HTML and PDF full-text extraction), and statutory citation verification across all major AI clients (**ChatGPT Desktop, OpenAI Codex CLI, Claude Desktop, Claude Code CLI, Cursor, Windsurf, VS Code / GitHub Copilot / Cline / Roo Code, Google Antigravity / Gemini CLI, Perplexity, and Continue.dev**).

---

### Interactive Desktop Setup (Select Your AI Assistant)

This package includes a graphical installer for legal practitioners and non-technical users that lets you select which AI application(s) you use:

1. **Download:** Click **`<> Code`** at the top right of this repository, select **`Download ZIP`**, and extract the folder to your computer.
2. **Run the Setup Utility:**
   - **Windows:** Double-click `Click_Here_To_Install_Windows.bat`
   - **macOS:** Double-click `Click_Here_To_Install_Mac.command`
3. **Select Your AI Client(s) & Connect:** Check the box(es) for the AI assistant(s) installed on your computer (**ChatGPT Desktop & OpenAI Codex CLI**, **Claude Desktop & Claude Code CLI**, **Cursor**, **Windsurf**, **VS Code / GitHub Copilot / Cline / Roo Code**, **Google Antigravity / Gemini CLI**, or **Perplexity / Continue.dev**), click **Install to Selected AI Clients**, and restart your selected AI application.

**System Integrity Note:** The setup utility operates strictly in read-only mode with respect to your personal files and documents. It installs an isolated Python runtime inside the extracted folder and registers the server entry only in the AI client configuration files you select.

---

### Multi-Tier Judicial Hierarchy & Live Indexed National Archives

This server performs live queries across the full judicial hierarchy and official legal archives of **Serbia**, extracting full text from both HTML pages and official court/gazette PDF judgments:

| Judicial Tier | Covered Courts & Tribunals |
|:---|:---|
| **Tier 1 — First Instance** | Osnovni sudovi (66 Basic Courts), Viši sudovi (25 Higher Courts in first-instance jurisdiction), Privredni sudovi (16 Commercial Courts) & Prekršajni sudovi |
| **Tier 2 — Regional / Cantonal / Appellate** | 4 Apelaciona suda (Beograd, Novi Sad, Niš, Kragujevac), Viši sudovi (appellate jurisdiction), Privredni apelacioni sud & Upravni sud Republike Srbije |
| **Tier 3 — Supreme & Constitutional** | Vrhovni sud Republike Srbije (vrhovni.sud.rs) & Ustavni sud Republike Srbije (ustavni.sud.rs) |

#### Official Portals & Live Indexed Domains

- **National Legislation & Official Gazette:** Pravno-informacioni sistem Republike Srbije (pravno-informacioni-sistem.rs) — [https://www.pravno-informacioni-sistem.rs](https://www.pravno-informacioni-sistem.rs)
  - *Indexed Legislation Domains:* `pravno-informacioni-sistem.rs`, `parlament.gov.rs`, `paragraf.rs`
- **Court Decisions & Jurisprudence Archives:** Pravno-informacioni sistem RS - Baza sudske prakse (pravno-informacioni-sistem.rs) & Portali Apelacionih Sudova — [https://www.pravno-informacioni-sistem.rs/SlGlasnikPortal/sudska-praksa](https://www.pravno-informacioni-sistem.rs/SlGlasnikPortal/sudska-praksa)
  - *Indexed Judicial & Open Case Law Domains:* `vrh.sud.rs`, `vrhovni.sud.rs`, `sudskapraksa.sud.rs`, `ustavni.sud.rs`, `pravno-informacioni-sistem.rs`, `paragraf.rs`, `bg.ap.sud.rs`, `ns.ap.sud.rs`

---

### Available MCP Tools

| Tool | Description |
|:---|:---|
| `search_legislation` | Searches enacted statutes, codes, decrees, and official gazette publications in Serbia. |
| `search_case_law` | Searches national jurisprudence and open judicial archives for Serbia. |
| `search_tiered_court_decisions` | Filters case law specifically by judicial instance (`first_instance`, `appellate_regional`, `supreme_constitutional`) or specific regional/cantonal/district court. |
| `list_court_hierarchy` | Returns the complete 3-tier court structure and supported regional court filters for Serbia. |
| `get_legal_document_markdown` | Retrieves full statutory or judicial texts (both HTML and official `.pdf` court judgments) and converts them into clean Markdown. |
| `verify_citation` | Validates statutory and case law citations against official registries. |

---

<details>
<summary><b>Manual Configuration for Developers (Optional)</b></summary>

```json
{
  "mcpServers": {
    "rs-legal-mcp": {
      "command": "uvx",
      "args": [
        "--from",
        "https://github.com/jurisatlas/rs-legal-mcp/archive/refs/heads/main.zip",
        "rs-legal-mcp"
      ]
    }
  }
}
```
</details>
