# 5-Day Evidence-Production Sprint Status

> **Sprint Goal:** Produce high-signal artifacts (Case Study + Demo Video, OpenWorldEye deployment + GIF, Spatial Agents public repo + GIF) and unlock Profile README (`chama-x/chama-x`).

---

## Sprint Overview & Acceptance Criteria

| Goal | Target Asset | Acceptance Criterion | Status |
| :--- | :--- | :--- | :--- |
| **UNLOCK-1** | `chama-x/case-studies` | Repo public, embedded 60s demo video (≤10MB mp4), sanitized screenshots, real metrics, written client permission confirmed | 🟡 In Progress (Permission GRANTED) |
| **UNLOCK-2** | `OpenWorldEye` Live | Deployed live (Vercel/Netlify) handling rate-limits gracefully, 30s GIF (≤10MB), logged-out smoke tested | 🔴 Cloned, Ready for Day 2 |
| **UNLOCK-3** | `spatial-agents` Public | Repo public, secrets-scan passed, clean README + 30s demo GIF (≤10MB) | 🔴 Ready for Day 3/4 |
| **PROFILE** | `chama-x/chama-x` README | All 3 unlock blocks uncommented with real URLs, zero HTML comments remaining, links verified logged-out | 🟡 Ready (Email set, awaits assets) |

---

## Day Plan & Task Checklist

### Day 1: Case Study Draft + Permission Request
- [x] **Agent:** Draft client permission request message ([client-permission-request.md](file:///Users/chamaththiwanka/Desktop/0/Projects/chama-x/drafts/client-permission-request.md)).
- [x] **User:** Send permission request / confirm client status (**GRANTED**).
- [ ] **Case Study Draft & Demo Video:** *On hold until user initiates.*
- [ ] **User:** Provide operational numbers & anecdote in `FACTS` block (when ready).
- [ ] **Agent:** Finalize the ~1,200-word case study draft based strictly on verified FACTS.
- [ ] **User:** Screen-record 60–90s demo (3D diorama + lorry states + Typst ticket compilation with dummy data).
- [ ] **Agent:** Compress demo recording to ≤10MB mp4.

### Day 2: OpenWorldEye Deployment
- [x] **Agent:** Clone OpenWorldEye locally ([openworldeye](file:///Users/chamaththiwanka/Desktop/0/Projects/openworldeye)).
- [x] **Agent:** Audit OpenWorldEye repo, configure `vercel.json` API proxy rewrites (CelesTrak, ADSB, ACLED) & fallback routing.
- [x] **Agent:** Format `openworldeye/README.md` to sprint structure.
- [x] **User/Agent:** Deploy to Vercel production (`https://openworldeye.vercel.app`).
- [x] **Agent:** Logged-out smoke test of the live URL (CelesTrak SGP4 satellite stream and ADSB radar proxy confirmed returning live data).

### Day 3: OpenWorldEye GIF & Spatial-Agents Prep
- [x] **Agent:** Run comprehensive secrets scan on `spatial-agents` repo (confirmed `.env` is git-ignored, no tracked keys).
- [x] **Agent:** Create sanitized `.env.example` for `spatial-agents`.
- [x] **Agent:** Draft `spatial-agents` public README ([spatial-agents/README.md](file:///Users/chamaththiwanka/Desktop/0/Projects/spatial-agents/README.md)).
- [ ] **User:** Record 30s screen capture of the live OpenWorldEye globe ([https://openworldeye.vercel.app](https://openworldeye.vercel.app)).
- [ ] **Agent:** Convert and optimize OpenWorldEye recording to GIF (≤10MB, 12fps, 800px wide).

### Day 4: Spatial-Agents Public & Case-Study Finalization
- [ ] **User:** Review and approve `spatial-agents` README.
- [ ] **User:** Record 30s screen capture of `spatial-agents` simulation.
- [ ] **Agent:** Convert and optimize `spatial-agents` GIF (≤10MB).
- [ ] **User:** Toggle `spatial-agents` GitHub repo visibility to Public.
- [ ] **Agent:** Finalize `case-studies` repo with compressed demo video, sanitized screenshots, verified metrics (when initiated).

### Day 5: Unlock & QA Gate (Non-Negotiable)
- [ ] **Agent:** Update `chama-x/chama-x` README — uncomment UNLOCK-1, UNLOCK-2, UNLOCK-3 with real URLs; remove all HTML comments.
- [ ] **Agent/User:** Logged-out browser smoke test across all visible links (ViT, case-studies, OpenWorldEye live, spatial-agents, etc.).
- [ ] **Agent/User:** Asset verification (ensure all videos, GIFs, screenshots render cleanly under size limits).
- [ ] **User:** Voice pass — read public copy aloud; simplify any flagged lines.
- [ ] **User:** Set GitHub pinned repos (`case-studies`, `spatial-agents`, `openworldeye`, `launchpad`) and update profile bio.

---

## Log & Updates

- **Day 1 Init:** Initialized `sprint-status.md` and set email `chamaththiwanka@icloud.com` in `README.md`.
- **Client Permission:** Confirmed GRANTED by Chamath.
- **Repos Verified:** `blackrock-ops`, `spatial-agents`, `openworldeye` (cloned), `case-studies` (scaffolded).
- **Case Study:** Paused locally per user instruction until explicitly initiated.
- **Profile Layout Refined:** Removed artificial SVG banner for a clean, human-first typographic layout leading directly into the 2×2 project evidence grid. Live demo links and verified email active.
