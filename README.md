# London Blue Plaques

An iOS app that transforms 413 curated English Heritage blue plaques in Central London into personal, AI-curated encounters with the city's history. Built in days with Claude Code and Figma MCP.

It's not information. It's an encounter.

<img width="1200" height="750" alt="discover_mode" src="https://github.com/user-attachments/assets/9879a4cc-e5f8-45fc-99f9-e9d4e92ec2db" />


---

## The Experience

London is full of blue plaques marking where remarkable people once lived and worked. Most people walk right past them. This app changes that.

Tell Claude what interests you, or just say "surprise me," and it curates a walking tour from wherever you're standing. Each stop is framed around your interests: a maths enthusiast gets Turing's theoretical work; a social justice lens gets the persecution and pardon story. The AI doesn't just retrieve information. It edits, frames, and personalizes it for you.

And at select stops, historical figures speak to you directly. Bertrand Russell looks into the camera and says: *"If your machines can learn knowledge, can they learn pity? That is the only question that matters."* These aren't generic audio guides. They're personal encounters that leave a mark.

<!-- SCREENSHOTS: Explore view + proximity nudge + detail page -->

---

## Bringing Figures to Life

Claude scripts what each figure says. Not filler dialogue, but cross-temporal conversations where historical figures address today's biggest questions from their own philosophical perspective. Turing on building minds versus soldiers. Keynes on the anxiety of freedom. Russell on decisions made by something never asked to care.

The cinematographic direction is deliberate: locked-off camera, Arri Alexa Mini aesthetic, BBC documentary colour grade, Kodak 5219 film stock. Claude and I developed the prompts together in Figma Weave (Veo 3), iterating on reference images, scene descriptions, and negative prompts until each generation felt right. Premiere Pro for the final polish.

This is deliberately pushing the boundaries of what's possible today. Some generations are stunning. Some hit the limits of current models. But the experience of a historical figure speaking to you at their own front door is so compelling that the limitations feel temporary. What's a stretch goal now may be routine in 12-18 months.

<img width="1200" height="914" alt="figmaWeave_Russell" src="https://github.com/user-attachments/assets/c41a0e5b-fce3-4df2-89b2-d2827d1c4f42" />

---

## From Wizard to One-Shot

The first version of Walk Planner was a three-step wizard: Where are you? What are you interested in? How long do you have? It was a standard UX pattern, and it failed. Too much friction, too many taps before anything happened.

The breakthrough was realizing the wizard existed because the app had no context. Claude has context. Version 2 replaced the entire wizard with a single prompt, or no prompt at all. The app knows where you are, it learns what you love, and it nudges you gently when you're within 50 meters of a plaque that matches your interests.

> "Curating your walk... Finding the perfect stops"

One input. One moment of anticipation. Then a fully curated walk with a title, a narrative, and a route mapped across London.

We curated the dataset down to 413 plaques in Zone 1, filtering out entries without portraits, outside Central London, or minor figures, to prioritize density and performance. Each plaque was enriched with gender and category data so Claude can intelligently match interests to figures. Ask for "Women who changed London" and the app knows exactly who qualifies and where they are.

<img width="1200" height="750" alt="one_shot_curation" src="https://github.com/user-attachments/assets/19e786c3-b875-4246-92f9-1e8047f6bc14" />


---

## Human + AI Collaboration

Sometimes Claude's routes zig-zag across the map, making a 60-minute walk into a 90-minute one. The order of stops matters as much as the selection, and AI doesn't always get it right.

The solution came from a real collaboration. Claude identified the problem (stop order won't always be optimal). I had the UX instinct (let the user drag and drop the cards). Claude extended the idea (update the map with renumbered stops in real time). Neither of us had the full solution alone.

This is how I think about AI in creative tools: not autonomous, not passive. Collaborative. AI proposes, human refines, the system adapts.

<!-- SCREENSHOTS: walk stop cards with drag handles + map before/after reorder -->

---

## What's Next

**Conversational AI at each stop** — Chat with Claude about any figure from the detail page. Ask about a figures friends or where they drank a pint. Ask what Turing might have accomplished with AI. Extend the "story" in history.

**Audio-first, eyes-free mode** — A gentle chime and on-device TTS as you walk: *"You're near 2 Warrington Crescent. Alan Turing lived here."* Heads up, earbuds in, glance down and hit the audio button for a brief synopsis about that person.

**My Plaques collection** — For collectors around the globe, blue plaques hold intrigue and challenge. Visiting a plaque in person automatically saves it to your collection. Users can share both walks and collected plaques with others. Should English Heritage decide to offer events and competitions, that's possible too.

**Cultural data as AI capability** — These plaques aren't just app content. They're a structured cultural dataset that becomes exponentially more valuable when exposed as AI capabilities via MCP. This prototype is a proof of concept for how any cultural institution could unlock their collections.

---

## See It for Yourself

Screenshots tell part of the story. To appreciate the sensation of 'meeting' historical figures (and hearing them speak), a live demo is available on request. Get in touch at elizmyers@gmail.com.

---

## Built With

Claude Code · Figma MCP · Figma Weave (Veo 3) · Adobe Premiere Pro · React Native / Expo · TypeScript

---

*Built by [Liz Myers](https://github.com/LizMyers) and Claude. I had the vision. Claude called it "the largest outdoor museum without an audio guide." We built it together.*
