# ⚡ Curlywerx — Modern AI Template Vault & Prompt Studio

**Curlywerx** is a production-grade, offline-first Android application designed for prompt engineers, researchers, and creators. Organize, customize, and execute AI prompts across any major LLM engine in seconds with dynamic placeholder variables and built-in Claude prompt synthesis.

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

### 📂 Organization, Search & Favorites
* Categorize templates into Coding, Writing, Productivity, Marketing, Audio, Video, Streaming, or custom categories.
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
* **Networking & JSON:** Kotlinx Coroutines, Android Networking, JSON serialization
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

* **Latest APK (v1.7.0):** `Curlywerx-v1.7.0-debug.apk`
* **Complete Source Code (v1.7.0):** `Curlywerx-v1.7.0-source.zip`

---

## 🔍 How to Check Your Current Version in the App

1. Open **Curlywerx**.
2. Tap the **Settings** icon (`⚙️`) in the bottom navigation bar or top right.
3. Scroll down to the bottom **About Curlywerx** card.
4. The **Version** row displays the live installed version and build number, e.g.:
   ```
   Version: v1.7.0 (Build 9)
   ```

---

## 📝 Changelog / Version History

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

