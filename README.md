# Proteus website, option 9 "CHANGE SHAPE. GET TO WORK." (final candidate)

## Figure-inspired design study

Local styling experiment in `assets/css/figure-study.css`, loaded after the original
stylesheet in `index.html`. The study uses lighter typography, a full-screen hero,
an editorial grid, off-white evidence sections and muted olive backgrounds. All
media and fonts remain self-hosted Proteus assets. Navigation and hero copy are
shortened; evidence labels and technical content are retained.

To return to the original styling, remove the `figure-study.css` stylesheet link.
The study has not been pushed or deployed.

Reading order: hero → problem → mission film and phases → prototype evidence and
team-background logos → module → physics → applications and Stage 1 specifications
→ mission and vision → founders film and biographies → contact. The route diagram
follows the mission phases. Reordering retains all existing content and media.

Preview from this directory with `npx vite --host 127.0.0.1 --port 4173` (Vite
provides HTTP range requests for video seeking).

Final combination (22 Oct 2026): v8 film and mission story, real hardware first, sourced problem, the shift, physics, the module, Stage 1 first job, plan, team. Dark story sections, light evidence sections. Built to replace the outis-robotics.com home page; /lab/ and /demo/ stay as they are. Static site: no build step, no cookies, no tracking, no third-party requests. Fonts are self-hosted.

| Path | Content |
|---|---|
| `index.html` | Hero film, key numbers, the problem (sourced), the mission film and six chapters, the readout, why modular (comparison), the module, proof and roadmap, go-to-market, team, contact |
| `impressum.html`, `privacy.html` | Legal pages (German) |
| `404.html` | Not-found page (absolute paths assume the site is served at `/proteus_9/`) |
| `assets/css/site.css` | Design tokens, components, layout |
| `assets/js/main.js` | Nav, film player, lazy looping clips with pause controls, readout typing, reveals |
| `assets/fonts/` | Archivo and IBM Plex Mono (SIL Open Font License 1.1) |
| `assets/media/` | v8 film, hero montage, chapter loops with posters, prototype clips, lab sheets |

Evidence labels: amber = render of MK3 target capability, green = lab statics on the exact MK1.1 kinematics, orange = real prototype.
Problem figures link to their sources (SES Ukraine via UNN, NIOSH 86-110, SES via Babel, Interfax-Ukraine).

## Local preview

Video needs a server with HTTP range support for Safari:

```bash
python3 ~/Proteus/Claude_Mission30/tools/range_server.py ~/Sites 8095
# open http://127.0.0.1:8095/proteus_9/
```
