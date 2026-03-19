# AI Agents Showcase

A one-page website showcasing student-built ElevenLabs Conversational AI agents.

## How to add/edit agents

Open `index.html` and find the `agents` array (around line 210). Each agent looks like this:

```js
{
  name: "Alex Morgan",         // Student's agent name
  role: "Career Coach",        // Short description
  tag: "Coaching",             // Badge label
  agentId: "AGENT_ID_1",       // ← paste ElevenLabs Agent ID here
  avatar: "https://..."        // URL to avatar image (or local path)
}
```

### Getting the Agent ID from ElevenLabs

1. Go to [elevenlabs.io](https://elevenlabs.io) → **Conversational AI** → **Agents**
2. Open the agent
3. Copy the **Agent ID** from the URL or the agent settings panel
4. Paste it as `agentId` in the array above

### Using a custom avatar image

Replace the `avatar` URL with:
- A direct image URL (jpg/png/webp), or
- A local file path like `"avatars/anna.jpg"` (place the file in an `avatars/` folder next to `index.html`)

---

## Publishing to GitHub Pages

1. Create a new repository on GitHub (e.g. `ai-agents`)
2. Upload `index.html` (and any `avatars/` folder) to the repo
3. Go to **Settings → Pages → Source: Deploy from branch → main → / (root)**
4. Your site will be live at `https://YOUR-USERNAME.github.io/ai-agents/`

---

## Adding more agents

Simply add more objects to the `agents` array — the grid adjusts automatically.
