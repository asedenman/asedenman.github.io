
## HM Land Registry RAG Q&A (private repository)

![Top language](https://img.shields.io/badge/python-100%25-3572A5)

A retrieval-augmented generation (RAG) application in Python that answers questions about HM Land Registry processes, grounded strictly in retrieved guide text with practice-guide citations — never the model's own knowledge. Covers the full pipeline: scraping the official GOV.UK collection, cleaning and chunking messy PDF and HTML sources, embedding into a vector store, and serving answers through a local chat interface.

- Ingests difficult real-world sources: scanned PDFs, header/footer cleanup, and section-aware HTML parsing.
- Guards retrieval quality with an evaluation gate against a golden question set, plus build versioning and a fully mocked, keyless test suite.
- Provider-agnostic config with swappable LLM/embedding backends (Anthropic, OpenAI, local HuggingFace).
- Built with Python, LangChain, ChromaDB, Gradio, BeautifulSoup, pypdf, and pytest.



## PdfBundler: [Source](https://gitlab.com/ased43/PdfBundler)

![Top language](https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fgitlab.com%2Fapi%2Fv4%2Fprojects%2Fased43%252FPdfBundler%2Flanguages&query=%24%5B%22C%23%22%5D&label=C%23&suffix=%25)

A .NET 10 application that consolidates multiple PDF files into a professionally formatted court bundle, producing a title page, a clickable table of contents, section-scoped page numbering (A1, A2, B1…), stamped page headers, bookmarks, and named destinations. Hosted on GitLab.

- A command-line interface for batch-processing bundles ([Link](https://gitlab.com/ased43/PdfBundler/-/blob/master/PdfBundler.Cli/Program.cs)).
- A two-phase bundling engine built on iText ([Link](https://gitlab.com/ased43/PdfBundler/-/blob/master/PdfBundler.Core/Bundler.cs)), shared between the CLI and an ASP.NET Core web API.
- Unit tests with xUnit ([Link](https://gitlab.com/ased43/PdfBundler/-/tree/master/PdfBundler.Tests)).


## Battery Modelling Notebook

![Top language](https://img.shields.io/github/languages/top/asedenman/BatteryModelling)

A demonstration Jupyter notebook created to show a possible application of machine learning to optimise a battery control system.
Uses Pandas and Numpy to shape data, and Keras to train a DQN model in order to minimise power costs by peak-shifting grid load.

- Data exploration and rough DFS search ([Link](https://github.com/asedenman/BatteryModelling/blob/master/Batteries.ipynb))
- Broad written analysis and Keras model ([Link](https://github.com/asedenman/BatteryModelling/blob/master/BatteryModel.ipynb))

## Turn-Based RPG — Godot 4 / C# (private repository)

![Top language](https://img.shields.io/badge/C%23-100%25-178600)

A turn-based RPG with a visual-novel overworld, built in Godot 4 (.NET) with C#. The core design principle is a strict separation between engine and content: all gameplay content — skills, enemies, status effects, events, dialogue, items — is authored as data (typed Resource definitions with stable string ids), loaded and validated at boot, keeping content production independant of code.

- Battle logic is a plain C# state machine that resolves synchronously and emits presentation cues consumed by an async presenter — presentation never mutates game state, and combat rules are unit-testable headlessly outside the engine.
- Effects are polymorphic data-driven definitions executed as a list; enemy AI is weighted intent scripts, with no specific enemy code.
- Single source of truth game state in a serialisable POCO, with a typed C# event bus for game logic and scene routing kept separate from overlay UI.
- Saves are versioned JSON via System.Text.Json.
- Character appearance is composed layer-by-layer from a single skeletal rig, derived directly from game state so visuals and mechanics cannot desync.
- Developer tooling first: an in-game debug console and loud-failing content validation were the earliest build targets.


## Mods for Rimworld:

Both these mods use a runtime patching library called Harmony. They are hosted on a separate GitHub account.

### NightVision: [Steam Workshop](https://steamcommunity.com/sharedfiles/filedetails/?id=1464989530&searchtext=) | [Source](https://github.com/AndTheManDrew/NightVision/tree/master/NightVision/Source) | [Youtube review](https://www.youtube.com/watch?v=5lTOfqgUMMo)

![Top language](https://img.shields.io/github/languages/top/AndTheManDrew/NightVision)

Approximately 2000 Steam subscribers.

Extends the light/dark mechanic from the base game. Affects combat, AI, character stats and gear, and in-game events.

- Detects all compatible game objects including other modded content ([Example](https://github.com/AndTheManDrew/NightVision/blob/master/NightVision/Source/ModInit/Init_Hediffs.cs)).
- Customises the results of the game's random character generator ([Link](https://github.com/AndTheManDrew/NightVision/blob/master/NightVision/Source/Incidents/SolarRaid_PawnGenerator.cs)) with xml output for testing ([Link](https://github.com/AndTheManDrew/NightVision/blob/master/NightVision/Source/Testing/DebugFlareRaidPawnGenXml.cs)).
- Dynamically patches methods depending on the users settings choices ([Example](https://github.com/AndTheManDrew/NightVision/blob/master/NightVision/Source/Settings/SettingOption.cs)).



### SquadUITweaks: [Steam Workshop](https://steamcommunity.com/sharedfiles/filedetails/?id=1455382219) | [Source](https://github.com/AndTheManDrew/SquadUITweaks/tree/master/Source)

![Top language](https://img.shields.io/github/languages/top/AndTheManDrew/SquadUITweaks)

Approximately 3000 Steam subscribers.

A simple QoL mod. Tweaks part of the game's UI by decorating a base game class with a callback.


## C++ Learning Project: [Source](https://github.com/asedenman/cpp_learning_project/tree/master/ProjectEuler/src)

![Top language](https://img.shields.io/github/languages/top/asedenman/cpp_learning_project)

A project for learning C++ by answering problems from projecteuler.net. Includes a win32 GUI.

- A custom window procedure ([Link](https://github.com/asedenman/cpp_learning_project/blob/master/ProjectEuler/src/windows/ProblemWindow.cpp)).
- Using memoisation to cut down problem solving time ([Link](https://github.com/asedenman/cpp_learning_project/blob/master/ProjectEuler/src/problems/Prob15.cpp)).
- Unit tests ([Link](https://github.com/asedenman/cpp_learning_project/blob/master/UnitTests/ProblemTests.cpp)).
