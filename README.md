# Flexible for Spryker

> **Unofficial** third-party plugin - not affiliated with or endorsed by Spryker.

## Core Features

### Transfer Objects
* **Completion, hover docs, and validation** for every element and attribute of the Transfer XSD in `.transfer.xml` files
* **Rename and Find Usages** for transfer names and properties across the whole project
* **Attribute value validation** against the Spryker Transfer schema, with quick fixes for common mistakes
* **Structure view, code folding, and brace matching** for fast navigation inside large transfer definitions
* **Picking a completion item** leaves a finished element behind, not an open tag waiting for a closing bracket

### OMS State Machines
* **Graph preview editor** with card-style state nodes, curved routed edges, drag, pan, and mouse-wheel zoom
* **PNG export** of the rendered state machine for documentation and reviews
* **Click-to-navigate** between a node in the preview and its definition in the XML
* **Context-aware completion** that only offers elements valid at the caret position and closes the tag for you
* **Go to Class** includes OMS processes alongside PHP classes
* **Isolated parse recovery**, so one broken process no longer breaks the preview for the rest of the file

### Propel Schema
* **Completion and validation** for `.schema.xml` files, including attribute names and column types
* **Foreign key and naming checks** that flag references and columns that do not follow Propel conventions
* **Documentation on hover** for every element and attribute defined by the Propel XSD
* **Structure view** for quick navigation through tables, columns, and relations

### Configuration Files
* **deploy.yml** - completion for application, region, and store values, with validation against the deploy schema
* **navigation.xml** - controller and bundle navigation, with a check for links that point nowhere
* **codeception.yml and tooling.yml** - completion and hover documentation
* **Glossary** - key navigation and completion, so translation keys resolve like any other reference
* **Config constants** - navigation to the defining class, plus checks for unknown constants and missing `getenv` guards

### PHP Integration (PhpStorm only)
* **DependencyProvider completion and checks** for provided and injected dependencies
* **Bridge and Facade sync checks**, with an intention to create a missing factory method
* **Constants navigation** from usage to declaration across the module tree
* **Extend core class in project** opens the existing override, or scaffolds one when none exists
* **Twig navigation** resolves component functions and template paths back to their source

### Docker and Debugging Tools
* **Docker SDK environment control** from a status bar widget, an environment tab, or the Tools > Spryker menu
* **One console per command**, with rerun and stop, instead of silent background execution
* **Xdebug remote debugging** with Docker path mapping and a single toggle to start listening
* **Cachegrind profiler** with a call tree and an icicle chart for reading where time went
* **Codeception test tree and run configurations**, with environment-state checks before a run starts

### Module Browser
* **Installed, project, and catalog views** for browsing Spryker modules in one panel
* **New Spryker Module action** with layer selection for scaffolding a module in the right place
* **Module detail panel** showing what is installed and what is available to add

## Getting Started

### Quick Start
1. Install the plugin from JetBrains Marketplace
2. Open a project that has `composer.json` identifying it as a Spryker project
3. The plugin detects the framework automatically and offers a guided tour
4. Set the Docker SDK path at **Settings > Tools > Flexible for Spryker**
5. Open the **Spryker** tool window from the right sidebar to browse modules and manage the environment
6. Open a `.transfer.xml`, OMS, or `.schema.xml` file and press **Ctrl+Space** for completion

### Productivity Tips
* **Ctrl+Q** on any Transfer, OMS, or Propel element for hover documentation with a link to the matching XSD
* **Click a state** in the OMS preview to jump straight to its definition in the XML
* **Alt+Enter** on an inspection warning for a quick fix
* **Live templates** speed up new transfer, state, and schema definitions
* **The status bar widget** gives one-click access to the running environment's commands

### Troubleshooting
* **No Spryker tool window?** The plugin only activates for a project with a Spryker `composer.json`
* **Debugger or tests will not start?** Start the Docker SDK environment first; the plugin reports when it is stopped instead of failing silently
* **Profiler panels stay empty?** Open a cachegrind file from the environment's profiler output to fill the call tree and icicle chart
* **PHP completion missing?** DependencyProvider, Bridge, and Facade checks need PhpStorm; they do not run in IntelliJ IDEA Community

## Compatibility

Works with:
* **IntelliJ IDEA** (Community or Ultimate) 2023.3+ - Transfer, OMS, and Propel XML support, the module browser, and Docker SDK and Xdebug control
* **PhpStorm** 2023.3+ - everything above, plus the PHP integration features (DependencyProvider, Bridge/Facade sync, constants navigation)

Built against IntelliJ Platform build 233 or newer.

## What's New in 2026.1.0

- Redesigned OMS preview with card-style nodes, routed edges, node drag, wheel zoom, and PNG export
- DependencyProvider completion and checks, plus Bridge signature sync and a factory-method intention, in PhpStorm
- Glossary key navigation and completion, alongside Codeception and Twig navigation
- deploy.yml, navigation.xml, codeception.yml, and tooling.yml completion, documentation, and broken-link checks
- Attribute value validation against the Transfer, OMS, and Propel XSDs, with quick fixes across all three languages
- Live environment status in the status bar, an environment tab, and one console per Docker SDK command
- Module browser rebuilt with installed, project, and catalog views, plus a New Spryker Module action
- Welcome dialog, guided tour, and a Getting Started tab with a live setup checklist

See [CHANGELOG.md](../CHANGELOG.md) for complete details.

## Made by Developers Who Ship Spryker Commerce Projects

The integration is the work of [Ilscipio](https://www.ilscipio.com/):

<p style="text-align:center">
<img src="https://www.ilscipio.com//wp-content/uploads/2018/11/ilscipio_soldier2-2.svg" width="200" alt="The Ilscipio Logo - A roman soldier"/>
</p>

We build and maintain Spryker shops for our clients and understand the daily grind of editing transfer definitions, state machines, and Propel schemas by hand. We created this plugin to bring real IDE support to that workflow.

We're sharing this tool with the Spryker community to support the ecosystem's growth and to help teams ship commerce projects with fewer detours into generated code and XML.

* Special discounts are available for individual developers and of course for the whole Open Source community.

## Links

* [JetBrains Marketplace](https://plugins.jetbrains.com/plugin/33832-flexible-for-spryker)
* [GitHub](https://github.com/ilscipio/flexible-spryker)

## Bugs & Feature Requests

If you have any questions, feature requests or stumble upon the occasional bug, please open an issue on [GitHub](https://github.com/ilscipio/flexible-spryker/issues) or reach out to us at [Ilscipio](https://www.ilscipio.com/).
