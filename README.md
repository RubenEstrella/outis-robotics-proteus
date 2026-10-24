# Proteus website, option 9 "CHANGE SHAPE. GET TO WORK." (final candidate)

## Figure-inspired design study

Local styling experiment in `assets/css/figure-study.css`, loaded after the original
stylesheet in `index.html`. The study uses lighter typography, a full-screen hero,
an editorial grid, off-white evidence sections and muted olive backgrounds. All
media and fonts remain self-hosted Proteus assets. Navigation and hero copy are
shortened; evidence labels and technical content are retained.

To return to the original styling, remove the `figure-study.css` stylesheet link.
The original design and ordering checkpoint is saved on GitHub as `0316f24`.

Reading order: vision hero -> original scrolling logo band -> problem -> first
market and planned business model -> prototype evidence -> force/configuration
targets -> execution milestones -> long-term miniaturization -> module details ->
mission concept -> team -> contact.
The three additional mission clips stay in a disclosure. The robot comparison is
always visible. The previously removed Stage 1 specifications table remains absent.
The execution and business sections are based on the v18 Track 2 work plan and
commercial path: qualification, integration, full-mission testing; paid feasibility
campaigns, module kits/integration, then service and calibration. Goals are not
presented as existing revenue, customers, qualified performance or funding secured.

The hero uses the existing concept rendering embedded in SPRIND v18, Appendix C.8:
`word/media/image1.jpg`, retained as `assets/media/vision-modules.jpg`. The inline
SVG viewport presents the visionary half of the original comparison without
altering the source bitmap. The full comparison is shown in section 06.
It is a concept rendering, not an engineering-checked configuration.

The three size halvings within five years are the founder's new long-term ambition,
requested on 24 October 2026, not a commitment quoted from the application.
The 1 -> 1/2 -> 1/4 -> 1/8 graphic describes relative linear dimensions. The
application supports the smaller-module direction and compact MK4 as its first
step; it does not establish force retention or full mission capability at those
future scales. The original mission film remains in section 08.

Force claims in section 04 are grounded in the Track 2 Metric 1 table and
Appendix C of `Proteus_SPRIND_Track_2_v18.docx` in Google Drive (file ID
`1-cr8YWCEUrYWhGTMxcmubyQcL6ojlLfr`). The nominal 10.20 ratio is the
200 N development target divided by the Reach Alpha 5 published 19.6133 N
lift-load equivalent; it is not an experimentally demonstrated improvement.
The previous 35x/560x comparison and illustrative load-path schematic have
been removed.
The adjacent configuration metric shows the founders' current target of 200+
physically validated configurations, confirmed by the user on 23 October 2026.
The v18 document specifies a minimum of 3 classes with at least 50 configurations
each (150 total minimum), not an upper limit. The Stage 1 interim goal remains
2 classes and 4 configurations. These are development targets, not current
validated counts.

Section 02 follows the v18 Track 2 work plan and customer/application descriptions.
The former three-equipment-mock-up hall and Stage 2 plant-partner wording came
from the Track 1 answers included in the same document. Track 2 Stage 1 instead
plans the magazine-chain-braced-working-structure-return segment on a test rig.
Application benefits and further markets are described as goals/planned uses.

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
