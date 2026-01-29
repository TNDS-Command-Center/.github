# TNDS Command Center

> AI-Powered Operations Framework + Google Apps Script Modules for Service Businesses

**"We don't just build systems. We put clients in command of their operations."**

**True North Strategy Ops** | jacob@truenorthstrategyops.com | www.truenorthstrategyops.com

---

## What Is This?

TNDS Command Center is a comprehensive operations framework combining:

1. **Claude Skills** — AI-powered methodologies for decision-making, sales, and delivery
2. **Command Protocol Installer** — 20+ Google Apps Script modules for client automation

Together, they form a complete system for running service business operations.

---

## Part 1: Claude Skills Framework

### The Six Skills

| Skill | Purpose |
|-------|---------|
| **Bearing Check** | 8-checkpoint decision validation framework |
| **Direction Protocol** | 5-stage client acquisition process |
| **Command Protocol** | 12-phase client delivery system |
| **World Model Mapper** | Deep operational process analysis |
| **ARO Assessment** | Agent-Ready Operations evaluation |
| **Documentation** | Professional document creation |

### Core Philosophy

**Direction Protocol gets you clarity. Command Protocol gets you control.**

*That's how we turn data into direction.*

---

## Part 2: Command Protocol Installer

A collection of modular Google Workspace automation tools for client deployments.

### Quick Start - GUI Installer (Recommended)

The easiest way to deploy modules is using the Command Protocol Installer - a desktop application with a graphical interface.

**Running the Installer:**
```
C:\temp\command-protocol-build\win-unpacked\Command Protocol Installer.exe
```

Or build/run from source:
```bash
cd installer
npm install
npm start          # Development mode
npm run dist:win   # Build distributable
```

**Important Note: Output Directory**

For reliable deployments, use an output directory outside of Windows-protected folders:
- **Recommended:** `C:\TNDS\deployments\` or `C:\Users\truenorth\Projects\`
- **Avoid:** Desktop, Documents, Downloads, OneDrive (Windows Defender may block hidden file writes)

### Command Line Deployment (Alternative)

**Option 1: Deploy Multiple Modules**
```bash
cd modules
node setup-all.js
```

**Option 2: Deploy Single Module**
```bash
cd modules/[module-name]
node setup.js
```

**Option 3: Config File Mode (Automation)**
```bash
cp modules/setup-config.example.json modules/setup-config.json
# Edit with your company info
cd modules
node setup-all.js --config setup-config.json
```

---

## Available Modules (20+)

### Core Tools

| Module | Description |
|--------|-------------|
| workspace-tools | Workspace Tools (Drive, Gmail, Calendar) |
| master-command | Central hub with GitHub integration |

### Industry-Specific

| Module | Description |
|--------|-------------|
| real-estate-command | Real estate automation suite |
| assetcommand | Fleet, asset & DOT compliance |

### Financial & Business

| Module | Description |
|--------|-------------|
| financial-command | Bank import, budgeting & AI categorization (v2.0) |
| tax-command | Tax tracking & CPA reports |
| contract-tracker | Contract management & renewal tracking |
| combined-fi-command | Multi-entity financial management |

### Automation & Workflows

| Module | Description |
|--------|-------------|
| proposal-generator-command | Automated proposal creation |
| onboarding-bot | Client provisioning system |
| office-automation | Reminders, Gmail labels, TNDS Tools |

### Addons & Integrations

| Module | Description |
|--------|-------------|
| command-center-addons | Email, calendar & search addons |
| looker-studio-command | Looker Studio dashboard integration |
| ui-command | White-label branding wizard |
| data-toolkit-command | Data cleanup & transformation |

### Government & Compliance

| Module | Description |
|--------|-------------|
| govcon-command | Federal contracts, SAM.gov, job boards |

### Analytics & SEO

| Module | Description |
|--------|-------------|
| seo-command | 9-command SEO audit workflow |

### Specialized (Non-Apps Script)

| Module | Description | Runtime |
|--------|-------------|---------|
| deck-command | Presentation builder | Next.js/Vercel |
| generate-presentation-command | README to HTML slides | Python |
| compliance-gov-module | SDVOSB compliance templates | Documentation |

---

## Documentation

| Document | Description |
|----------|-------------|
| docs/2026-01-28-USER-MANUAL.md | Complete user manual |
| docs/2026-01-28-MODULE-CATALOG.md | All modules detailed reference |
| docs/SPECIALIZED_MODULES.md | Non-Apps Script deployment guide |
| docs/CLIENT-DEPLOYMENT-GUIDE.md | Client site deployment instructions |
| DEVELOPMENT.md | Module development workflow |
| installer/README.md | Installer technical details |
| tests/MODULE-TEST-CHECKLIST.md | Module validation checklist |

---

## Folder Structure

```
TNDS-Command-Center/
├── Claude Skills/
│   └── Claude ai Skills/           # AI Skills Framework
│       ├── Bearing-Check-Skill/
│       ├── ARO-Assesment-Skill/
│       ├── World-Model-Mapper-Skill/
│       ├── Direction-Protocol-Skill/
│       ├── Command-Protocol-Skill/
│       ├── Documentation-Skill/
│       ├── WORKFLOW_INTEGRATION.md
│       └── USER-MANUAL.md
│
└── 10_COMMANDS/
    └── command protocol-installer/  # Module Installer
        ├── installer/               # GUI Installer (Electron app)
        │   ├── backend/             # Backend modules
        │   │   ├── orchestrator.js
        │   │   ├── clasp-manager.js
        │   │   ├── deploymentHistory.js
        │   │   ├── clientProfiles.js
        │   │   ├── versionManager.js
        │   │   └── backupManager.js
        │   ├── src/                 # React UI components
        │   ├── config/              # Module, template & version configs
        │   └── docs/                # Installer documentation
        ├── modules/                 # All deployable modules (20+)
        │   ├── workspace-tools/
        │   ├── real-estate-command/
        │   ├── financial-command/
        │   ├── proposal-generator-command/
        │   ├── tax-command/
        │   ├── govcon-command/
        │   ├── master-command/
        │   ├── seo-command/
        │   ├── deck-command/
        │   ├── compliance-gov-module/
        │   └── _shared/             # Shared utilities
        ├── docs/                    # Project documentation
        ├── archive/                 # Deprecated modules & old docs
        └── tests/                   # Test checklists & scripts
```

---

## Prerequisites

- Node.js v18+ ([download](https://nodejs.org/))
- Google clasp CLI: `npm install -g @google/clasp`
- Google Workspace account
- Apps Script API enabled: https://script.google.com/home/usersettings

### First-time Setup

```bash
npm install -g @google/clasp
clasp login
```

---

## Who Is This For?

- Operations consultants
- Service business owners
- Agencies serving SMBs
- Anyone building AI-augmented workflows

---

## Version History

### Claude Skills v1.0 (January 29, 2026)
- All 6 skills implemented
- Complete documentation and integration guides
- Workflow integration across all skills

### Command Protocol Installer v2.1.0 (January 29, 2026)
- Deployment History - Track all deployments with search, filter, and export
- Client Profiles - Save and reuse client configurations for quick re-deployment
- Module Update Checker - Compare deployed versions with current versions
- Backup Manager - Backup scripts before re-deployment with restore capability
- New tabbed UI: Deploy | History | Updates | Backups

### Command Protocol Installer v2.0.0 (January 28, 2026)
- Rebranded to "Command Protocol"
- 20+ modules across 9 categories
- Deprecated 7 legacy modules (migrated to -command naming)
- Added retry, log export, error catalog, and recovery features
- Fixed OAuth scopes in 4 modules
- Validated all module paths and files

### Command Protocol Installer v1.0.0 (January 4, 2026)
- Initial installer release
- 13 modules

---

## Support

**True North Strategy Ops**

- Email: jacob@truenorthstrategyops.com
- Web: www.truenorthstrategyops.com

---

## License

This is a private repository. All rights reserved.

Copyright 2026 True North Data Strategies, LLC

---

**Last Updated:** January 29, 2026

