# True North Data Strategies - Google Apps Script Command Modules

A complete collection of Google Workspace automation modules for business operations.

**Version:** 4.0 (January 2026)
**Total Modules:** 26+
**All modules production-ready with dashboards and automation**

---

## Complete Module Directory

| # | Module | Industry Focus | Description |
|---|--------|----------------|-------------|
| 1 | **ai-command** | Any | AI integration and automation tools |
| 2 | **analytics-command** | Any | Advanced analytics and reporting |
| 3 | **asset-command** | Fleet/Construction | Fleet and asset tracking with maintenance |
| 4 | **client-google-apps-module-setup** | Any | Client deployment and setup tools |
| 5 | **Combined Financial Center 2.1** | Finance/Accounting | Unified financial operations |
| 6 | **compliance-gov-module** | Government/Regulated | Government compliance tracking |
| 7 | **contract-command** | Any | Contract management and renewal alerts |
| 8 | **core-addons** | Any | Essential workspace utilities |
| 9 | **data-command** | Any | Data processing and cleanup tools |
| 10 | **deck-command** | Sales/Marketing | Presentation and deck automation |
| 11 | **family-command** | Personal | Family organization and scheduling |
| 12 | **financial-command-center** | Finance | Bank imports and budget tracking |
| 13 | **govcon-command** | Government | Government contracting operations |
| 14 | **installer** | Any | Module deployment and setup |
| 15 | **master-command** | Any | Orchestration and module coordination |
| 16 | **office-command** | Office Ops | Office automation and reminders |
| 17 | **onboard-command** | MSP/IT | Client provisioning and onboarding |
| 18 | **packaging-studio** | Product | Module packaging and distribution |
| 19 | **proposal-command** | Sales | Automated proposal generation |
| 20 | **realty-command** | Real Estate | Complete real estate operations |
| 21 | **seo-command** | Marketing | SEO tracking and optimization |
| 22 | **sms-command** | Communications | SMS integration and automation |
| 23 | **squirrel-command** | Development | Code utilities and dev tools |
| 24 | **tax-command** | Finance/Tax | Tax tracking with OCR receipts |
| 25 | **ui-command** | Design | UIUX tools and branding |
| 26 | **workspace-command** | Any | Workspace setup and organization |

---

## Quick Start

### Prerequisites

1. **Node.js** (v14 or higher) - [Download](https://nodejs.org/)
2. **Google clasp CLI**
   ```bash
   npm install -g @google/clasp
   clasp login
   ```
3. **Google Workspace** account

### Deploy Multiple Modules

Use the master installer for batch deployment:

```bash
cd installer
node setup-all.js
```

The installer will:
1. Collect your company information once
2. Identify your industry and recommend modules
3. Deploy selected modules with shared configuration
4. Set up integrations between modules
5. Create unified dashboards

### Deploy Single Module

```bash
cd [module-name]
node setup.js
```

### Config File Mode (Automation)

```bash
# Copy and customize template
cp setup-config.example.json setup-config.json

# Run batch deployment
node setup-all.js --config setup-config.json
```

---

## Module Details

### Core Operations Modules

#### **workspace-command**
Google Workspace foundation:
- Drive folder structure creation
- Gmail label management and auto-rules
- Daily email digest
- Lead capture from emails
- Workspace inventory and cleanup

**Best for:** Any business starting workspace setup.

#### **master-command**
Command orchestration:
- Cross-module coordination
- Unified dashboard aggregation
- Module health monitoring
- Centralized configuration
- Batch operations

**Best for:** Multi-module deployments.

#### **core-addons**
Essential utilities:
- Email notifications with templates
- Calendar integration
- Advanced search with saved queries
- Meeting scheduling
- Shared helper functions

**Best for:** Foundation for other modules.

---

### Industry-Specific Modules

#### **realty-command**
Complete real estate automation:
- Lead pipeline tracking
- Property listings management
- Transaction tracker with commission calculator
- Showing scheduler
- Calendar sync (Showings, Open Houses, Closings)
- Email follow-up automation
- MLS integration ready

**Compliance:** GLBA, Fair Housing Act, State Retention Laws

**Best for:** Real estate agents, brokerages, property managers.

#### **govcon-command**
Government contracting operations:
- SAM.gov integration
- Opportunity tracking
- Proposal coordination
- Past performance database
- Capability statement generator
- Teaming agreement tracker

**Compliance:** FAR/DFARS, NIST 800-171

**Best for:** Government contractors, SDVOSB/VOSB businesses.

#### **compliance-gov-module**
Government compliance management:
- Regulation tracking (FAR, DFARS, NIST)
- Audit trail logging
- Document retention policies
- Access control monitoring
- Compliance reporting

**Best for:** Regulated industries, government contractors.

---

### Financial & Tax Modules

#### **financial-command-center**
Core finance operations:
- Bank statement JSON import
- Auto-categorization of transactions
- Budget tracking and alerts
- Visual spending dashboard
- Multi-account support

**Best for:** Small businesses, freelancers.

#### **Combined Financial Center 2.1**
Unified financial operations:
- Integrates financial-command + tax-command
- P&L statement generation
- Cash flow forecasting
- Tax-ready reporting
- Accountant export formats

**Best for:** Established businesses needing complete financial visibility.

#### **tax-command**
Tax tracking system:
- Gmail receipt import
- PDF OCR processing
- Auto-categorization with rules engine
- AI categorization (OpenAI optional)
- MACRS depreciation calculator
- SDVOSB compliance checking
- CPA-ready PDF reports
- Schedule C preparation

**Best for:** Tax management, expense tracking, sole proprietors.

#### **contract-command**
Contract management:
- Contract list with 18+ data columns
- Renewal date tracking with alerts
- Expiration notifications (30/60/90 days)
- Document linking to Drive
- Dashboard with contract overview
- Vendor/client categorization

**Best for:** Any business with contracts, vendor management.

---

### Sales & Marketing Modules

#### **proposal-command**
Automated proposal generation:
- Google Form intake
- 5+ service-specific templates
- Automatic PDF generation (~80KB)
- Email delivery via Gmail
- Drive organization (Proposals, Templates)
- Tracking spreadsheet with Dashboard
- Win/loss analytics

**Best for:** Sales teams, consultants, agencies.

#### **deck-command**
Presentation automation:
- Slide template management
- Auto-population from Sheets
- Brand consistency enforcement
- Export to PDF/PPTX
- Version control

**Best for:** Sales teams, marketing, executives.

#### **seo-command**
SEO tracking and optimization:
- Keyword rank tracking
- Backlink monitoring
- Content optimization suggestions
- Competitor analysis
- Google Search Console integration
- Reporting dashboards

**Best for:** Marketing teams, agencies, content creators.

---

### Operations & Asset Modules

#### **asset-command**
Fleet and asset management:
- Vehicle/equipment/tool tracking
- Check-out/check-in logging
- Maintenance scheduling and alerts
- Cost tracking and analysis
- Visual dashboards (2 included)
- Daily digest emails
- QR code integration

**Best for:** Construction, rental businesses, fleet managers.

#### **office-command**
Office automation:
- Scheduled email reminders
- Gmail label management
- Sender-to-label mapping
- Automated trigger processing
- Task management integration

**Best for:** Office managers, assistants, operations.

---

### Client & Team Modules

#### **onboard-command**
Client provisioning automation:
- Google Workspace user provisioning
- Shared Drive creation
- Gmail label setup
- Document generation from templates
- AppSheet GUI interface
- Rollback capability
- Welcome email sequences

**Best for:** MSPs, IT consultants, agencies.

#### **client-google-apps-module-setup**
Client deployment tools:
- Module selection wizard
- Batch client setup
- White-label configuration
- Multi-tenant management
- Client portal generation

**Best for:** Service providers, MSPs, consultants.

---

### Data & Analytics Modules

#### **data-command**
Data utilities:
- Remove duplicates
- Trim whitespace
- Auto format
- Data validation
- Import/export tools
- Batch processing

**Best for:** Data operations, spreadsheet cleanup.

#### **analytics-command**
Advanced analytics:
- Custom metric tracking
- Trend analysis
- Predictive modeling
- Looker Studio integration
- Automated reporting
- KPI dashboards

**Best for:** Data-driven businesses, executives.

---

### AI & Automation Modules

#### **ai-command**
AI integration platform:
- OpenAI/Anthropic integration
- Document analysis
- Auto-categorization
- Content generation
- Smart routing
- Conversation logs

**Best for:** Businesses leveraging AI for automation.

#### **sms-command**
SMS automation:
- Twilio integration
- Two-way messaging
- Scheduled messages
- Template management
- Response tracking
- Contact sync

**Best for:** Customer service, sales teams, notifications.

---

### Development & Design Modules

#### **ui-command**
UIUX toolkit:
- Company editor with logo/colors
- Theme system (4+ default themes)
- Preview panel
- Branding profile management
- White-label capabilities
- Dashboard interface

**Best for:** Design teams, white-label deployments.

#### **squirrel-command**
Developer utilities:
- Code generation
- Script optimization
- Debug logging
- Performance monitoring
- Error tracking
- Development shortcuts

**Best for:** Apps Script developers, technical teams.

---

### Specialized Modules

#### **family-command**
Family organization:
- Shared calendar management
- Chore tracking
- Allowance tracking
- School schedule integration
- Family communications
- Event planning

**Best for:** Personal use, family organization.

#### **packaging-studio**
Module distribution:
- Module packaging
- Version control
- Distribution management
- Update deployment
- Documentation generation

**Best for:** Module developers, internal operations.

---

## Recommended Setup by Business Type

### Real Estate Agency
1. **realty-command** - Core operations
2. **workspace-command** - Foundation
3. **contract-command** - Contract management
4. **sms-command** - Client communications
5. **proposal-command** - Listing presentations

### Government Contractor (SDVOSB/VOSB)
1. **govcon-command** - Opportunity tracking
2. **compliance-gov-module** - Compliance management
3. **proposal-command** - Proposal automation
4. **contract-command** - Contract tracking
5. **workspace-command** - Foundation

### Construction / Fleet
1. **asset-command** - Asset tracking
2. **workspace-command** - Foundation
3. **contract-command** - Subcontractor management
4. **sms-command** - Crew communications

### Consulting / Agency
1. **proposal-command** - Client proposals
2. **onboard-command** - Client provisioning
3. **workspace-command** - Foundation
4. **contract-command** - Contract management
5. **deck-command** - Presentations

### Small Business (General)
1. **workspace-command** - Workspace setup
2. **financial-command-center** - Finance tracking
3. **tax-command** - Tax management
4. **contract-command** - Contract tracking
5. **office-command** - Daily operations

### Finance/Accounting Firm
1. **Combined Financial Center 2.1** - Complete finance ops
2. **tax-command** - Tax tracking
3. **contract-command** - Client contracts
4. **data-command** - Data cleanup
5. **workspace-command** - Foundation

### Marketing Agency
1. **seo-command** - SEO tracking
2. **proposal-command** - Client proposals
3. **deck-command** - Presentations
4. **analytics-command** - Campaign analytics
5. **workspace-command** - Foundation

### MSP / IT Consultant
1. **onboard-command** - Client provisioning
2. **client-google-apps-module-setup** - Multi-client deployment
3. **contract-command** - MSA tracking
4. **workspace-command** - Foundation

---

## Module Integration Matrix

Modules designed to work together:

| Primary Module | Integrates With | Benefit |
|----------------|-----------------|---------|
| realty-command | sms-command | Automated client texts |
| realty-command | proposal-command | Listing presentations |
| financial-command-center | tax-command | Tax-ready transactions |
| govcon-command | proposal-command | Government proposals |
| govcon-command | compliance-gov-module | Compliant operations |
| asset-command | sms-command | Maintenance alerts |
| onboard-command | workspace-command | Complete client setup |
| proposal-command | deck-command | Proposal presentations |
| analytics-command | ALL | Cross-module reporting |
| master-command | ALL | Unified orchestration |

---

## Feature Comparison Matrix

| Feature | Included In |
|---------|-------------|
| Dashboard | All modules |
| Function Runner | Most modules |
| Gmail Integration | workspace, office, realty, proposal, tax |
| Drive Integration | workspace, onboard, proposal, tax |
| Calendar Integration | realty, office, family |
| Lead Tracking | workspace, realty |
| Asset Tracking | asset-command |
| Bank Import | financial-command-center, Combined Financial 2.1 |
| Tax Tracking | tax-command, Combined Financial 2.1 |
| PDF Generation | proposal, onboard, tax, contract |
| OCR Processing | tax-command |
| AI Integration | ai-command, tax-command |
| SMS Integration | sms-command |
| Government Features | govcon-command, compliance-gov-module |
| White-Label | ui-command, client-google-apps-module-setup |
| Analytics | analytics-command |
| SEO Tools | seo-command |

---

## Security & Compliance

All modules follow True North Data Strategies security standards:

**Default Protections:**
- Least privilege access
- Encryption in transit/at rest
- Secure logging (no PII in logs)
- Input validation
- Error handling

**Compliance-Ready Modules:**
- **govcon-command**: FAR/DFARS, NIST 800-171
- **compliance-gov-module**: FedRAMP considerations
- **realty-command**: GLBA, Fair Housing Act
- **tax-command**: IRS regulations
- **financial-command-center**: SOC2-aligned
- **All modules**: GDPR, CCPA/CPRA data handling

For government work, modules flag FedRAMP, NIST 800-53, and FISMA considerations.

---

## Installation & Support

### Standard Installation
```bash
# Clone repository
git clone https://github.com/truenorthdata/command-modules.git
cd command-modules

# Install dependencies
npm install

# Run setup wizard
cd installer
node setup-all.js
```

### White-Label Deployment
For MSPs and consultants deploying to multiple clients:
```bash
cd client-google-apps-module-setup
node white-label-setup.js
```

### Module Updates
```bash
# Update all modules
cd installer
node update-all.js

# Update specific module
cd [module-name]
git pull
clasp push
```

---

## Development

### Creating Custom Modules

Use `packaging-studio` to scaffold new modules:
```bash
cd packaging-studio
node create-module.js
```

### Module Standards
All Command modules follow:
- Naming: `[name]-command` format
- Structure: Dashboard, Function Runner, Config
- Documentation: README, CHANGELOG, setup.js
- Testing: Test functions in each module
- Logging: Logger.log() for debugging

### Contributing
1. Fork repository
2. Create feature branch
3. Follow coding standards
4. Submit pull request

---

## Pricing & Licensing

**Individual Modules:** $500-2,500 per module
**Industry Bundles:** $3,000-7,500 (3-5 modules)
**Complete Suite:** Contact for enterprise pricing
**White-Label Rights:** Available for MSPs

All modules include:
- Setup and configuration
- 30-day support
- Documentation
- Updates for 1 year

---

## Support & Resources

**True North Data Strategies**
- Email: jacob@truenorthstrategyops.com
- Phone: 719-204-6365
- Web: truenorthstrategyops.com
- Location: Colorado Springs, CO

**Documentation:**
- [User Manual](docs/USER-MANUAL.md)
- [Module Catalog](docs/MODULE-CATALOG.md)
- [Compliance Checklist](docs/COMPLIANCE-CHECKLIST.md)
- [API Reference](docs/API-REFERENCE.md)
- [White-Label Guide](docs/WHITE-LABEL-GUIDE.md)

**Training:**
- Video tutorials: youtube.com/@truenorthdata
- Written guides: docs.truenorthstrategyops.com
- Live training: Available for bundles

---

## Roadmap

**Q1 2026:**
- Mobile app integration (AppSheet)
- Enhanced AI features across modules
- Salesforce connector
- QuickBooks integration

**Q2 2026:**
- Microsoft 365 compatibility layer
- Advanced analytics dashboards
- Multi-language support
- API marketplace

**Q3 2026:**
- Industry-specific AI agents
- Predictive maintenance (asset-command)
- Lead scoring (realty-command)
- Contract AI review (contract-command)

---

## About True North Data Strategies

**Mission:** Turn data into direction for small businesses.

**Tagline:** Enterprise-grade automation for businesses that existed before iPhones.

**Certifications:** SBA-certified VOSB/SDVOSB

**Owner:** Jacob Johnston
- 20-year Army veteran (Airborne Infantry)
- Service-disabled veteran
- Bronze Star recipient
- Google Workspace automation specialist

**Service Delivery:**
- **Command Center Build** - $2,500-5,000, 2-4 weeks
- **Battle Rhythm Install** - $2,000-4,000, 2-4 weeks  
- **Command Partner** - $1,000-2,000/month (ongoing support)

---

## License

Copyright © 2026 True North Data Strategies LLC
All rights reserved.

Individual module licenses available.
White-label licensing available for MSPs and consultants.

---

**Last Updated:** January 25, 2026
**Version:** 4.0
**Total Modules:** 26+
**Status:** Production Ready
