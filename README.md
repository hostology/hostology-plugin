# Hostology

The Hostology plugin for Claude and ChatGPT lets a venue set itself up in [Hostology](https://hostology.co.uk) by
talking to its AI assistant. It brings two things:

- **The Hostology venue connector**, which lets the assistant read your venue's setup and add your catalogue,
  pricing, payment terms and workflows for you.
- **The Hostology Onboarding skill**, which walks you through your venue's setup checklist: where you have got to,
  what comes next, the work the assistant can do with you, and where in the venue portal to do the rest.

## What you need

- A Hostology venue account.
- AI assistant access switched on for your venue. A venue admin turns it on in the venue portal, under
  Application Settings -> AI assistants.

## Install

**Claude:** find Hostology in Claude's plugin directory and install it. In Claude Code you can also install it
from this repository:

```
/plugin marketplace add hostology/hostology-plugin
/plugin install hostology@hostology
```

**ChatGPT:** find Hostology in ChatGPT's plugin directory and install it.

When you connect the plugin, you sign in through Hostology and approve the assistant's access to your venues. Then
ask: "Help me set up my venue".

## Privacy

Hostology's privacy policy: https://hostology.co.uk/privacy/

## Licence

MIT. See [LICENSE](LICENSE).
