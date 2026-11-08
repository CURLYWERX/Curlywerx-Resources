# ⚡ Curlywerx — Modern AI Template Vault & Prompt Studio

**Curlywerx** is a production-grade, offline-first Android application designed for prompt engineers, researchers, and creators. Organize, customize, and execute AI prompts across any major LLM engine in seconds with dynamic placeholder variables and built-in prompt synthesis.

---

## ✨ Features

### 🧩 Dynamic Placeholder Variables
* **Standard Variables:** Standard dynamic placeholders like `{{topic}}` or `{{code}}` work seamlessly, supporting spaces and descriptive names (e.g. `{{Streaming Service}}`, `{{Topic or Concept}}`).
* **Option Choices (Single-Line Horizontal Scroll):** Provide quick 1-tap choice chips using the pipe `|` syntax:
  * `{{Tone|Professional, Casual, Academic, Witty}}`
  * `{{Format|Bullet Points, Table, Essay, Step-by-Step}}`
* **Default Value Syntax:** Pre-fill input fields with sensible defaults using colon `:` syntax:
  * `{{word_count: 800-1200}}`
  * `{{Tone: Professional | Casual, Firm, Persuasive}}`
* **Pre-Selected Default Option:** Use `*` to pre-select a specific option from the choice list on initial load:
  * `{{Tone|*Professional, Casual, Academic}}` (marks *"Professional"* as the active choice)
* **Live Dynamic Form Generation:** Responsive fill-in forms dynamically generate input fields and interactive chips for each detected variable.
* **Real-time Preview:** Instantaneous token replacement, word/char counts, and clipboard copy.

### 🚀 1-Tap Multi-Engine Web Execution
* Run filled prompts directly into your favorite AI engine with one click:
  * **ChatGPT** (`chatgpt.com`)
  * **Claude** (`claude.ai`)
  * **Google Gemini** (`gemini.google.com`)
  * **Perplexity AI** (`perplexity.ai`)
  * **DeepSeek** (`chat.deepseek.com`)
  * **Grok** (`x.com/i/grok`)
  * **Microsoft Copilot** (`copilot.microsoft.com`)
  * **Mistral Le Chat** (`chat.mistral.ai`)
  * **Poe** (`poe.com`)
  * **HuggingChat** (`huggingface.co/chat`)
* **Custom Engines:** Add custom web endpoints or company AI portals in Settings.

### 🪄 Universal AI Prompt Engineer (Multi-Engine)
* Synthesize high-performing prompt templates tailored with variables for any goal:
  * **User-Selectable AI Engine:** Choose your default prompt architect in Settings or switch on the fly: Anthropic Claude, OpenAI ChatGPT, Google Gemini, DeepSeek, Perplexity AI, or xAI Grok.
  * **Direct API Mode:** Connect your Anthropic, OpenAI, Google Gemini, or DeepSeek API key for instant, automated prompt synthesis directly in-app.
  * **1-Tap Web Mode:** Launch your chosen AI web portal with pre-engineered meta-prompts automatically copied to your clipboard (zero API key required), then parse the response with 1 tap.
  * **Offline Blueprint Mode:** Instant rule-based prompt synthesis that works offline without an internet connection.

### 🌐 Online Prompt Marketplace & Remote CDN Library
* **1-Tap Community Hub:** Access the online prompt library directly from the Home top bar (`LocalLibrary` icon).
* **Zero Rate Limits via CDN:** Fetches remote prompt catalogs and packages asynchronously via high-speed jsDelivr CDN caching (`https://cdn.jsdelivr.net/gh/CURLYWERX/Curlywerx-Resources@main/marketplace_catalog.json`), completely bypassing GitHub API rate limits.
* **Prompt Packs & Single Templates:** Preview and install individual templates or multi-prompt packs with 1-tap installation directly into Room SQLite with conflict-free deduplication.
* **Resilient URL Fallback & Casing Engine:** Auto-resolves URL directory casing and provides transparent fallback to raw GitHub endpoints.

### 🌿 Built-in Botanical Category & Image Analysis
* **Universal Visual Botanical Profiler:** Field botanist, toxicologist, and ethnobotanist image-analysis template featuring household safety profiles, geographic location grounding, matching strictness, and medical disclaimers.
* **Wild Edible Plant Foraging Guide:** Vascular plant foraging, edibility and utility matrices, pathogen and toxin safety processing rules, and ethical harvesting protocols.
* **Weed & Pest Diagnostic Guide:** Agronomic visual inspection protocol with organic, biocontrol, chemical, and IPM treatment methodologies.

### ⚡ Technical Maker & Media Built-in Blueprints
* **Hardware Pinout & Wiring Reference:** Development board reference (Arduino Uno/Nano/Mega, ESP32-C3/S3, Raspberry Pi 4/5/Pico) with component pinouts, communication protocols, and safety validation.
* **Linux Terminal Command Finder:** Instant shell/terminal command solver across Raspberry Pi OS/Debian, Ubuntu Server, and Alpine Linux with safety notes and syntax flags.
* **Streaming Content Curator:** High-fidelity entertainment recommendations with chronological ordering, 38+ categorized genres, and 8+ major streaming service integrations.

### 📂 Organization, Search & Favorites
* Categorize templates into Coding, Writing, Productivity, Marketing, Audio, Video, Streaming, Botanical, or custom categories.
* **Dynamic Custom Categories:** Any custom category entered when creating a template is instantly registered in the global category manager, database table, and Home filter chips.
* **Strict Alphabetical AI Engine Ordering:** All default and user-added custom AI engines (e.g. Mistral, Copilot, Cohere) are automatically alphabetized across all pickers and menus.
* Instant fuzzy search across titles, template bodies, and hashtags (`#tags`).
* Star templates as favorites with dedicated one-tap filter toggling.

### 💾 Backup, Restore & Privacy
* 100% offline-first local database powered by Android **Room**.
* Full JSON export and import for seamless cross-device migration and backups.
* No personal data or prompts leave your device without your explicit action.

---

## 🛠️ Architecture & Tech Stack

* **Language:** 100% Kotlin
* **UI Toolkit:** Jetpack Compose with Material Design 3 (M3)
* **Architecture:** MVVM (Model-View-ViewModel) + StateFlow
* **Database:** Android Room with KSP
* **Networking & CDN:** OkHttp, Coroutines, jsDelivr CDN, GitHub Raw fallback
* **AdMob & Monetization:** Rewarded Ad slot unlock system + Google Play Billing foundation
* **Compatibility:** Android 8.0+ (API 26+)

---

## 🎨 Brand Assets & Icons

Curlywerx features a distinctive developer-first brand identity built around the visual language of nested curly braces `{{ }}` and dynamic prompt variable compilation.

| Asset | Resolution | Purpose | Location |
| :--- | :--- | :--- | :--- |
| **Android Adaptive Launcher** | 108dp Safe Zone / Mipmap | Android OS Home Screen & App Drawer | `res/mipmap-*/ic_launcher.png`, `ic_launcher_round.png` |
| **GitHub Avatar / Profile** | 512 × 512 (Circular Masked) | GitHub Organization / Repo Icon | `art/curlywerx-github-avatar-512x512.png` |
| **Play Store / Store Listing** | 512 × 512 | Google Play Console Store Icon | `art/curlywerx-icon-512x512.png` |
| **Master High-Res Brand Icon** | 1024 × 1024 | Hi-Res Vector/Digital Exports | `art/curlywerx-icon-1024x1024.png` |
| **Multi-Scale Icons** | 256, 128, 64, 32 px | Documentation, Web Favicons & Badges | `art/curlywerx-icon-*x*.png` |

---

## 📦 Downloads & Releases

* **Latest APK (v1.9.0):** `Curlywerx-v1.9.0-debug.apk`
* **Complete Source Code (v1.9.0):** `Curlywerx-v1.9.0-source.zip`
* **Previous APK (v1.8.0):** `Curlywerx-v1.8.0-debug.apk`
* **Previous Source (v1.8.0):** `Curlywerx-v1.8.0-source.zip`

---

## 🔍 How to Check Your Current Version in the App

1. Open **Curlywerx**.
2. Tap the **Settings** icon (`⚙️`) in the bottom navigation bar or top right.
3. Scroll down to the bottom **About Curlywerx** card.
4. The **Version** row displays the live installed version and build number, e.g.:
   ```
   Version: v1.9.0 (Build 11)
   ```

---

## 📝 Changelog / Version History

### [v1.9.0] - (Build 11) - 2026-11-08
* **Online Prompt Library Marketplace:** Added TopAppBar marketplace action (`LocalLibrary` icon) connected to a public CDN repository to browse, preview, and 1-tap install community and expert prompt templates and prompt packs.
* **Rate-Limit-Free CDN Architecture:** Uses jsDelivr CDN (`cdn.jsdelivr.net/gh/CURLYWERX/Curlywerx-Resources@main/...`) for rapid cached downloads without hitting GitHub API limits.
* **Resilient URL & Casing Fallback:** Built-in auto-casing candidate resolution and raw GitHub fallback automatically handles directory casing differences on remote repositories.
* **Built-in Botanical Category & Prompts:**
  * Added new default category `"Botanical"`.
  * Added *"Universal Visual Botanical Profiler"* for computer-vision plant toxicity, taxonomy, and safety profile reports.
  * Added *"Wild Edible Plant Foraging Guide"* for vascular plant foraging and pathogen/toxin processing rules.
  * Added *"Weed and Pest Diagnostic Guide"* for agronomic pests with organic, chemical, and IPM treatment protocols.
* **Maker & Coding Blueprints:**
  * Added *"Hardware Pinout and Wiring Reference"* covering Arduino (Uno, Nano, Mega), ESP32 (C3, S3), Raspberry Pi (4, 5, Pico) pinouts, power calculations, and test firmware.
  * Added *"Linux Terminal Command Finder"* providing exact shell commands and syntax breakdowns across distributions.
* **Enhanced Streaming Content Curator:** Upgraded *"Streaming Content"* with 38+ categorized genres, multi-platform streaming selectors (Netflix, Hulu, Max, Prime Video, Disney+, Apple TV+, etc.), and chronological ordering.
* **Dynamic Custom Categories:** Adding a template with a custom category name automatically adds that category to the global database table and immediately displays it in Home filter chips and category pickers.
* **Strict Alphabetical AI Engine Ordering:** All default and user-added custom AI engines (e.g., Mistral, Copilot, Cohere) are strictly and dynamically sorted in alphabetical order.
* **Settings & About Updates:** Updated About card with Prompt Marketplace and Prompt Engineer info, and integrated v1.9.0 What's New release notes.

### [v1.8.0] - (Build 10) - 2026-10-08
* **Template Architect Variable Engine Alignment:** Upgraded the Universal Prompt Engineer (API, Web, and Offline synthesizer) to strictly follow the full mobile variable syntax specification.
* **Strict Variable Naming:** Variable placeholders generated by AI now strictly use underscores without spaces: `{{variable_name}}`.
* **Alphabetical Option Choice Chips:** Option choices `{{variable_name|Option1, Option2, ...}}` are strictly sorted alphabetically by AI with unlimited choices allowed.
* **Default Values & Pre-Selected Chips:** Pre-selects default options using asterisk syntax `{{variable_name|*Option1, Option2}}` in correct alphabetical position, and generates default values `{{variable_name: DefaultValue}}` or combined `{{variable: Def | Opt1, Opt2}}`.
* **Alphabetical AI Engine Selection:** The AI Engine switcher (Prompt Engineer screen & Settings) is strictly sorted alphabetically (`ChatGPT`, `Claude`, `DeepSeek`, `Gemini`, `Grok`, `Perplexity`). Any user-added custom engines (via Settings or the new `+ Add` button) are dynamically integrated in alphabetical order.
* **Comprehensive Multi-Engine System Prompts & Web Meta-Prompts:** Centralized architecture rules across Claude, OpenAI, Google Gemini, and DeepSeek direct APIs, as well as 1-tap browser web generation.
* **Rewritten Offline Blueprints:** Refactored built-in offline templates across Coding, Streaming, Marketing, Writing, Auto Repair, Culinary, Productivity, and Gaming to leverage choice chips, pre-selected defaults, and strict variable formatting.

### [v1.7.0] - (Build 9) - 2026-10-06
* **Live Word & Approximate Token Counter:** Added live `~150 Words • ~195 Tokens` badge to the template editor (`AddEditTemplateSheet`), the filled prompt preview (`TemplateDetailScreen`), and the Prompt Engineer synthesis preview to help users monitor model context window usage.
* **Universal Multi-Engine "Prompt Engineer":** Renamed "Claude Prompt Engineer" throughout the app to simply **"Prompt Engineer"**, and added support for user-selectable AI engines (Anthropic Claude, OpenAI ChatGPT, Google Gemini, DeepSeek, Perplexity AI, xAI Grok).
* **Live Engine Switcher Strip:** Switch between synthesis models directly on the Prompt Engineer screen with 1 tap.
* **Multi-Provider Direct API Mode:** Integrated direct API generation for OpenAI (GPT-4o), Google Gemini (1.5 Flash/Pro), DeepSeek (V3/Chat), and Anthropic Claude.
* **1-Tap Web Mode for All Engines:** One tap copies pre-engineered meta-prompts to the user's clipboard and launches the selected AI web portal with zero API key required.
* **Room Database v9 Migration:** Added database columns and migrations for `prompt_engineer_ai`, `openai_api_key`, `gemini_api_key`, and `deepseek_api_key`.

### [v1.6.0] - (Build 8) - 2026-10-04
* **Quick-Insert 3-Button Syntax Toolbar:** Added a permanent 3-button formatting bar right above the prompt editor to instantly insert or wrap text with `{ } {{var}}`, `{ : } {{var: def}}`, and `{ |* } {{Choice|*Opt}}` without digging through soft keyboard submenus.
* **Saved Named Variable Presets:** Save frequently used variable combinations as named presets (e.g., "Arduino Nano 115200", "Formal Pitch") for instant 1-tap reuse with deletion & preview support.
* **Recent Executions History (Last 5 Runs):** Automatically tracks and stores the last 5 executed/copied prompts per template. View history, copy exact output, or 1-tap restore all variable inputs.
* **Seamless In-Memory Active Draft Retention:** User inputs are automatically cached across screen navigations so switching between screens never loses dynamic inputs.
* **Room Database v8 Migration:** Added local SQLite tables and indices for `prompt_presets` and `execution_history` with full schema migration.

### [v1.5.0] - (Build 7) - 2026-10-04
* **Horizontal Scroll for Variable Choices:** Converted dynamic variable choice chips to a single-line horizontal scroll (`Row` + `horizontalScroll`) to prevent long option lists (such as 13+ Arduino boards) from elongating the page.
* **Scroll Affordance:** Added an indicator badge (`X choices • Scroll ↔`) when more than 3 options are available.
* **Unified APK Launcher Icon:** Restored the authentic launcher icon to the main screen top bar and About card.
* **Top Bar Declutter:** Streamlined top bar header to maximize horizontal screen space.

### [v1.4.0] - (Build 6)
* **Variable Dropdown Choice Syntax:** Added support for double-brace options `{{Variable|Option 1, Option 2}}` with default markers `*`.
* **AdMob Monetization & Premium Slots:** Integrated Google Mobile Ads SDK with rewarded ad slots and slot counter cards.
* **Compact / Detailed View Toggle:** Added home screen view density toggle.

### [v1.3.0] - (Build 5)
* **Claude AI Prompt Engineer:** Integrated prompt generation via Anthropic API, Claude Web meta-prompts, and offline blueprints.
* **Multi-Engine Execution:** Added support for launching filled prompts across 10+ AI web engines.

