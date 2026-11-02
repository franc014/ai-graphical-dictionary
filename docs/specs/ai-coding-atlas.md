# AI Coding Atlas

## Problem Statement

Developers adopting AI-assisted coding face a fragmented vocabulary. Definitions alone do not show how models, context, harnesses, tools, sessions, failure modes, handoffs, memory, and human workflows affect one another in practice. Existing written references are useful for lookup, but they do not provide the visual mental models, guided progression, interactive practice, or durable feedback needed to apply and diagnose these concepts during real software work.

The product must make the concepts explorable as a dictionary and learnable as a connected curriculum. It must remain technically trustworthy, visually engaging, fast, private, and useful without an account. It must also avoid copying prose or editorial arrangement from Matt Pocock's unlicensed `dictionary-of-ai-coding` repository.

## Solution

Build **AI Coding Atlas**, a static-first interactive learning website for experienced developers who are new to AI coding. The site will independently explain all 71 factual concepts identified during research, reorganized into six original laboratory zones. It will combine a searchable dictionary, a readable 2.5D relationship atlas, guided learning paths, interactive lessons, authored scenario quizzes, and a browser-local Lab Notebook.

Fifteen foundational concepts will receive deep, 8–12 minute flagship lessons. The remaining concepts will receive original 2–4 minute mini-lessons. Every lesson will include a graphical explanation, concrete example, related concepts, primary-source citations, a visible verification date, and at least one authored knowledge check. Five conceptual systems will receive selective Three.js scenes; precise instructional diagrams will otherwise use accessible SVG and HTML enhanced by GSAP explanatory motion.

The experience will use a playful tactile-laboratory identity without sacrificing editorial clarity. It will be deployable as a static Astro site to Cloudflare Pages, use Plausible for anonymous aggregate learning events, and keep all personal progress in the learner's browser.

## User Stories

1. As a developer new to AI coding, I want a clear explanation of the field's vocabulary, so that I can communicate precisely with teammates.
2. As a developer, I want concepts organized around a coherent mental model, so that I understand how individual terms fit into a working system.
3. As a first-time visitor, I want a clear starting point, so that I can begin learning without deciding among 71 terms.
4. As a first-time visitor, I want to preview the site's teaching style from the homepage, so that I can decide whether the experience is relevant to me.
5. As a learner, I want a foundations path, so that I can study core concepts in a sensible prerequisite order.
6. As a learner with a specific question, I want to browse the dictionary freely, so that I do not have to follow the course sequence.
7. As a learner, I want all lessons to remain unlocked, so that guidance never becomes an artificial barrier.
8. As a learner, I want prerequisite cues and recommended next steps, so that open exploration still has direction.
9. As a learner, I want section-based mini-paths, so that I can focus on one area after completing or skipping the foundations path.
10. As a visitor, I want the product's purpose and intended audience stated clearly, so that I know what background knowledge is assumed.
11. As a visitor, I want a concise explanation of the site's relationship to Matt Pocock's dictionary, so that the inspiration and independent authorship are transparent.
12. As a visitor, I want an About and Sources area, so that I can understand the editorial and evidence standards.
13. As a reference user, I want fuzzy search across term names and descriptions, so that I can find a concept even when I do not know its exact title.
14. As a reference user, I want to filter terms by laboratory zone, depth, mastery, and relationship, so that I can narrow the index quickly.
15. As a learner, I want to switch between a conventional list and a relationship atlas, so that I can choose the representation that suits my task.
16. As a keyboard user, I want to search, filter, and open terms without a pointer, so that the core reference experience remains operable.
17. As a learner, I want the atlas to show all 71 concepts, so that I can see the breadth of the domain.
18. As a learner, I want the atlas to focus on one concept's neighborhood, so that the full network does not become unreadable.
19. As a learner, I want labeled relationship paths, so that a connection communicates meaning rather than mere proximity.
20. As a learner, I want pan, zoom, focus, and reset controls in the atlas, so that I can navigate it deliberately.
21. As a learner, I want atlas search results to move focus to the matching concept, so that search and spatial exploration reinforce one another.
22. As a mobile learner, I want the atlas to remain readable and controllable on a small screen, so that it is not a desktop-only novelty.
23. As a learner, I want flagship lessons to begin with why the concept matters, so that the detail has an immediate practical purpose.
24. As a learner, I want each flagship lesson to establish one concise mental model, so that I retain a usable explanation.
25. As a learner, I want a guided visual demonstration, so that dynamic systems are easier to understand than through prose alone.
26. As a learner, I want concrete coding-agent examples, so that I can transfer the concept into real work.
27. As a learner, I want common misconceptions called out explicitly, so that I can replace incorrect assumptions.
28. As a learner, I want each lesson to show related concepts, so that I can expand my understanding contextually.
29. As a learner, I want a lesson summary before assessment, so that I can consolidate the mental model.
30. As a learner, I want primary sources available from the lesson, so that I can verify claims and study further.
31. As a time-constrained learner, I want mini-lessons to take only 2–4 minutes, so that every indexed term is still useful at launch.
32. As a mini-lesson reader, I want an original definition, practical importance, compact visual, concrete example, and quick-check, so that short entries still teach rather than merely label.
33. As an experienced developer, I want explanations to assume software-development fluency, so that lessons do not repeat basic programming material.
34. As a learner, I want examples to be vendor-neutral by default, so that the concepts remain useful as products change.
35. As a learner, I want named products used only when they clarify a real implementation, so that examples remain concrete without becoming marketing.
36. As a learner, I want concise, direct writing with light playfulness, so that the material feels approachable without losing precision.
37. As a learner, I want a related term's definition previewed on hover or focus, so that I can resolve a small knowledge gap without leaving the lesson.
38. As a learner, I want to inspect a related term in a side panel, so that I can see its compact visual and immediate relationships without losing my place.
39. As a mobile learner, I want related-term details in a bottom sheet, so that the interaction fits the available viewport.
40. As a learner, I want an explicit action to open the related term's full lesson, so that navigation remains intentional.
41. As a learner, I want my current lesson position preserved after closing a related-term panel, so that exploration does not disrupt learning.
42. As a learner, I want selected concepts represented as tactile 3D systems, so that invisible processes become memorable spatial models.
43. As a learner, I want 3D scenes to guide me through authored states, so that free camera movement does not obscure the explanation.
44. As a curious learner, I want limited optional orbit or drag exploration after a guided step, so that I can inspect the system myself.
45. As a learner on a low-power device, I want 3D scenes loaded only when needed, so that the rest of the site remains fast.
46. As a learner without WebGL, I want an equivalent 2D explanation, so that lesson meaning is not dependent on rendering support.
47. As a motion-sensitive learner, I want motion reduced or replaced according to my system preference, so that the site remains comfortable to use.
48. As a learner, I want animation to demonstrate state changes and flows, so that motion carries instructional meaning.
49. As a learner, I want explicit step controls for complex animations, so that I can advance, reverse, or replay an explanation at my own pace.
50. As a reader, I want scroll-triggered motion used sparingly, so that scrolling remains predictable and content remains readable.
51. As a learner, I want one authored quick-check for every mini-lesson, so that every concept includes retrieval practice.
52. As a flagship learner, I want five varied scenario questions, so that assessment measures application rather than definition recall alone.
53. As a learner, I want immediate answer feedback, so that mistakes become learning opportunities while the reasoning is fresh.
54. As a learner, I want feedback to explain why alternatives are wrong, so that I can diagnose misconceptions.
55. As a learner, I want unlimited quiz retries, so that mastery is attainable without penalty.
56. As a learner, I want a lesson marked mastered after scoring at least 80%, so that mastery has a consistent meaning.
57. As a learner, I want viewed and mastered states distinguished, so that exposure is not confused with understanding.
58. As a learner, I want quiz content to be deterministic and editorially reviewed, so that grading is reliable.
59. As a privacy-conscious learner, I want quizzes to work without sending answers to an AI service, so that learning does not require disclosing activity.
60. As a returning learner, I want my progress restored in the same browser, so that I can continue where I stopped.
61. As a returning learner, I want zone and path progress summarized in a Lab Notebook, so that I can see what to learn next.
62. As a learner, I want completed experiments and mastery shown without points or streak pressure, so that progress feels informative rather than manipulative.
63. As a learner, I want to export my Lab Notebook as JSON, so that I can back up or move my progress without an account.
64. As a learner, I want to import a valid progress export, so that I can restore progress on another browser or device.
65. As a learner, I want invalid progress imports rejected with a useful explanation, so that corrupted data does not damage my notebook.
66. As a learner, I want to reset all local learning data deliberately, so that I retain control over information stored on my device.
67. As a privacy-conscious visitor, I want the site to avoid accounts and personal tracking, so that I can learn anonymously.
68. As a privacy-conscious visitor, I want analytics limited to aggregate learning events, so that product improvement does not require behavioral profiles.
69. As a learner, I want a light-first theme and an optional dark theme, so that I can choose a comfortable presentation.
70. As a learner, I want theme preference retained locally, so that the site remains consistent between visits.
71. As a reader, I want high-contrast text, visible focus, and semantic structure, so that the site remains legible and navigable.
72. As a screen-reader user, I want instructional graphics to have meaningful textual equivalents, so that essential lesson content is not image-only.
73. As a mobile learner, I want lessons, quizzes, navigation, panels, and notebook controls to adapt to small screens, so that all core workflows remain available.
74. As a learner, I want feedback and status changes announced accessibly, so that quiz and progress updates are perceivable without sight.
75. As a visitor, I want pages to load quickly on representative mobile hardware, so that rich visuals do not create a slow reference site.
76. As a visitor, I want nonessential 3D and animation code excluded from initial page loads, so that ordinary lesson reading stays lightweight.
77. As a search-engine user, I want each lesson to have a unique indexable page, so that I can discover a concept directly from search results.
78. As a visitor sharing a lesson, I want accurate titles, descriptions, and social metadata, so that the shared link communicates its value.
79. As a learner, I want a visible last-verified date, so that I can judge whether technical material may be stale.
80. As a learner, I want numbered references connected to an expandable source drawer, so that citations are available without interrupting reading.
81. As a maintainer, I want lesson metadata and required sections validated at build time, so that incomplete content cannot silently ship.
82. As a maintainer, I want all term identifiers and routes to be unique and stable, so that links and saved progress remain durable.
83. As a maintainer, I want broken concept relationships detected automatically, so that the atlas cannot point to missing terms.
84. As a maintainer, I want quiz answers and mastery rules validated, so that malformed assessment data cannot ship.
85. As a maintainer, I want citations and verification dates required, so that the evidence standard is enforced consistently.
86. As a maintainer, I want content authored in typed MDX collections, so that rich interactions and editorial validation can coexist.
87. As a maintainer, I want the taxonomy to be extensible beyond the initial 71 concepts, so that curated future snapshots do not require an architectural rewrite.
88. As a maintainer, I want source changes reviewed manually, so that external edits do not overwrite original teaching or introduce unverified claims.
89. As a maintainer, I want graphics to share reusable primitives and design tokens, so that 71 lessons remain visually coherent.
90. As a maintainer, I want 3D scenes to follow a common lifecycle and cleanup contract, so that navigation does not leak render loops or event handlers.
91. As a maintainer, I want anonymous learning events to use a documented event vocabulary, so that analytics remain intentional and comparable.
92. As a maintainer, I want production-like browser tests around critical learner journeys, so that refactors preserve behavior.
93. As a maintainer, I want content-contract tests independent of visual implementation, so that curriculum errors receive fast feedback.
94. As a maintainer, I want automated accessibility checks on representative pages and states, so that basic regressions are caught before release.
95. As a maintainer, I want the site deployable as static output, so that hosting remains inexpensive and operationally simple.
96. As a maintainer, I want canonical URL configuration centralized, so that a placeholder can be replaced safely when a domain is chosen.
97. As a maintainer, I want modern evergreen browser support defined explicitly, so that compatibility work has a clear boundary.
98. As a maintainer, I want code and content released under MIT, so that the project's reuse terms are explicit.
99. As a maintainer, I want the original inspiration credited in the About area and relevant lesson sources, so that provenance is transparent.
100. As a project owner, I want deployment to pause for explicit Cloudflare authorization, so that publishing never assumes access to external infrastructure.

## Implementation Decisions

### Product and editorial model

- The product name is **AI Coding Atlas**.
- The primary audience is experienced software developers who are new to AI coding.
- The product is a hybrid reference and course: all concepts remain freely browsable while learning paths provide guidance.
- All educational prose, examples, quiz questions, taxonomy descriptions, and graphics will be original. The source dictionary may be used as research input for factual concepts, but its prose and editorial arrangement will not be copied or closely adapted.
- The source inspiration will be credited in the About experience and where relevant in lesson source drawers.
- The editorial voice will be direct, precise, concise, and lightly playful. It will avoid hype and unnecessary anthropomorphism.
- Examples will be vendor-neutral by default. Named providers, models, or coding agents may appear when they clarify a concrete implementation and will be labeled as examples rather than canonical behavior.
- Technical claims will be verified against primary sources such as official documentation, specifications, or papers. Every lesson will expose sources and a last-verified date.
- Source updates will be reviewed as curated snapshots. There will be no automated synchronization with the external dictionary.

### Information architecture

- The compact top-level shell will include Home, Explore, Paths, term lessons, and About/Sources.
- The visible header will emphasize **Explore** and **Paths**, plus a global Lab Notebook progress control.
- Explore will combine two modes on one destination: a searchable/filterable dictionary list and a 2.5D relationship atlas.
- The Lab Notebook will be a global drawer rather than a standalone top-level destination. It will provide progress summaries and export, import, and reset controls.
- Every concept will have a stable, indexable lesson route with canonical metadata.
- The homepage's primary action will start the foundations path. Explore and atlas entry points will remain visible alternatives.

### Original laboratory taxonomy

- All 71 researched term concepts will ship in the initial index. The taxonomy will support adding original concepts in later curated snapshots.
- The concepts will be reorganized into six original zones with creative names and explicit descriptive subtitles:
  - **Model Engine — How generation works:** AI, Model, Parameters, Training, Inference, Effort, Token, Next-token prediction, Non-determinism, Model provider, Model provider request, Input tokens, Output tokens, Prefix cache, Cache tokens.
  - **Context Chamber — What the model can perceive now:** Stateless, Context, Context window, Stateful, System prompt, Session, Turn.
  - **Agent Workshop — How models act through software:** Harness, Agent, Environment, Filesystem, Tool, Tool call, Tool result, MCP, Permission request, Permission mode, Agent mode, Sandbox, Subagent.
  - **Reliability Observatory — Why outputs and long sessions fail:** Sycophancy, Hallucination, Parametric knowledge, Knowledge cutoff, Contextual knowledge, Attention relationship, Attention budget, Attention degradation, Smart zone.
  - **Continuity Lab — How work survives context boundaries:** Clearing, Handoff, Primary source, Secondary source, Handoff artifact, Spec, Ticket, Compaction, Autocompact, Memory system, AGENTS.md, Progressive disclosure, Context pointer, Skill.
  - **Human Control Room — How people steer and verify work:** Human-in-the-loop, AFK, Automated check, Automated review, Human review, Vibe coding, Design concept, Grilling, Prototyping, DX, AX, Software factory, Dark factory.

### Curriculum and lesson model

- Fifteen flagship lessons will form the initial foundations path in this order: Model; Token; Next-token prediction; Context; Context window; Model provider request; Harness; Agent; Tool call; Session; Non-determinism; Hallucination; Attention degradation; Compaction; Memory system.
- A focused flagship lesson will target 8–12 minutes. It will follow eight recurring stages: why it matters; mental model; guided visual; concrete example; misconception; related concepts; assessment; sources.
- The other 56 concepts will receive 2–4 minute mini-lessons. Each will contain an original definition, why it matters, a compact visual explanation, a concrete example, and one quick-check.
- Learning paths will include the flagship foundations path and zone-based mini-paths.
- Content will be authored as typed MDX collections so lessons can combine validated metadata, prose, and interactive components.
- Required metadata will include stable identity, title, concise description, zone, depth, relationships, prerequisites, learning outcomes, verification date, sources, visual type, quiz data, and estimated duration.

### Relationship and atlas interactions

- Related concepts will use progressive disclosure: hover or keyboard focus reveals a concise preview; activation opens a side panel; an explicit action navigates to the full lesson.
- On narrow screens, the related-term side panel will become a bottom sheet.
- Closing a preview will restore focus and preserve the learner's lesson position.
- The atlas will be 2D/2.5D rather than a true 3D network. It will prioritize readable labels and meaningful relationships while using depth, GSAP motion, focus transitions, pan, and zoom for spatial character.
- The atlas will show the complete network overview and support local-neighborhood focus to manage complexity.
- List and atlas modes will share search and filters. Search will be fuzzy across names and descriptions; filters will include zone, content depth, mastery state, and relationship context.

### Visual design and motion

- The visual identity will be a tactile toy laboratory: warm paper-like surfaces, dark ink text, cobalt, vermilion, yellow, mint, modular objects, connectors, labels, and dimensional shadows.
- The default presentation will be light-first with a complete optional dark theme. Theme preference will persist locally.
- Typography will pair a distinctive editorial variable sans with a monospaced face for system labels and mechanical details.
- Graphics will use a coherent visual grammar of tokens, containers, paths, gates, tools, context layers, state labels, and relationship lines.
- GSAP will be used for explanatory state transitions, sequencing, and restrained scroll reveals. Explicit controls will dominate complex teaching interactions; scroll will not be hijacked.
- The official GSAP skills will be installed globally before implementation. The existing Matt Pocock `teach` skill will be explicitly loaded when producing educational content.
- Five lazy-loaded direct Three.js system scenes will cover: generation mechanics; the context chamber; the agent/tool loop; attention degradation and compaction; and persistent memory systems.
- Three.js scenes will provide authored camera states with limited optional exploration. They will not become unrestricted 3D sandboxes.
- Precise instructional diagrams will use SVG and semantic HTML. Every WebGL scene will have an equivalent 2D representation for reduced motion, low capability, or rendering failure.
- Nonessential animation and 3D code will be loaded only where used and cleaned up when its host interaction is removed.

### Assessment and progress

- Quiz questions will be authored, deterministic, source-reviewed, and shipped with static content. The site will make no runtime model API calls.
- Each mini-lesson will include one quick-check. Each flagship lesson will include five varied questions emphasizing realistic scenarios, application, and misconception diagnosis.
- Feedback will be immediate and will explain both correct reasoning and relevant incorrect alternatives.
- Learners may retry without limit. A score of at least 80% marks a lesson mastered.
- Progress will distinguish **viewed/completed** from **mastered**. Completion reflects meaningful passage through the lesson interaction; mastery reflects the quiz threshold.
- All content will remain open regardless of progress or mastery.
- The Lab Notebook will visualize path, zone, completion, and mastery progress without points, leaderboards, streaks, or pressure mechanics.
- Personal progress and theme state will remain browser-local. Learners can export, import, and reset progress. Imports will be versioned and validated before changing stored state.

### Accessibility and responsive behavior

- Launch safeguards will include semantic HTML, keyboard operability, visible focus, sufficient contrast, accessible control names, status announcements, and reduced-motion support.
- Essential meaning will never exist only in animation, color, canvas, hover, or pointer interactions.
- Interactive graphics will provide textual equivalents. WebGL content will provide equivalent 2D teaching states.
- Panels and sheets will manage focus, restore focus on close, close predictably, and prevent background interaction when modal.
- Core navigation, lessons, quizzes, atlas controls, related-term exploration, and the Lab Notebook will work across mobile and desktop layouts.
- The target browser range is the current and previous major releases of Chrome, Safari, Firefox, and Edge.

### Technical architecture

- The application will use Astro with static output, typed MDX content collections, vanilla TypeScript interactive islands/custom elements, native CSS with cascade layers and design tokens, Three.js, and GSAP.
- No React, Vue, Svelte, hosted CMS, user-account service, application database, or runtime AI service will be introduced for the initial release.
- pnpm will manage dependencies and scripts.
- ESLint and Prettier will provide linting and formatting, including compatible handling for Astro and MDX content.
- Client state will use small framework-free modules with explicit serialization boundaries. The progress export format will include a schema version.
- The canonical site URL will be centralized behind placeholder configuration until a deployment URL or custom domain is approved.
- The project will generate sitemap, canonical metadata, social metadata, and structured data appropriate for indexable educational term pages.
- The initial release will be online-first and PWA-compatible in structure, but will not ship a service worker or offline cache.

### Analytics, performance, deployment, and licensing

- Plausible will collect aggregate page views and anonymous learning events for lesson starts, lesson completions, quiz mastery, atlas use, and path starts. Events will not include quiz answers, exported progress, personal identifiers, or free-form content.
- The performance target is a Lighthouse performance score of at least 90 on representative mobile hardware, alongside strong Core Web Vitals.
- 3D, atlas, and lesson-specific interaction code will be lazy-loaded. Rendering will favor transforms and opacity and avoid unnecessary layout or paint work.
- The production target is Cloudflare Pages. The implementation will produce a deployable static build and deployment configuration.
- Actual publication will pause for explicit Cloudflare authorization. No credentials or infrastructure access will be assumed.
- The project will be initialized as a local Git repository. A GitHub remote is not part of implementation unless separately authorized.
- Code and original educational content will be released under the MIT License.

## Testing Decisions

- Tests will assert externally observable behavior and durable content contracts, not internal component structure, private methods, CSS class names, animation frame values, or Three.js scene-graph implementation details.
- The project will use two primary test seams:
  1. **Built-site browser seam:** a production-like static build served locally and exercised with Playwright.
  2. **Content contract seam:** curriculum, assessment, relationships, and serialized progress validated at build/unit level with Vitest and Astro's content validation.
- Browser tests will cover the critical first-time path from homepage to the first foundations lesson, lesson progression, related-term preview/panel/full navigation, quiz feedback, mastery, Notebook updates, and resuming after reload.
- Browser tests will cover Explore list/atlas switching, fuzzy search, zone/depth/mastery filters, atlas focus, and opening a term from both modes.
- Browser tests will cover local progress export, valid import, invalid import rejection, and deliberate reset.
- Browser tests will cover light/dark theme persistence, narrow-screen panel behavior, keyboard navigation, focus restoration, and reduced-motion behavior.
- Browser tests will cover representative WebGL success and fallback behavior at the user-visible boundary rather than asserting renderer internals.
- Automated accessibility checks will run against representative shell, Explore, flagship lesson, mini-lesson, quiz feedback, panel/sheet, and Lab Notebook states. Keyboard-only flows will also be exercised explicitly.
- Content contract tests will require exactly 71 unique initial concepts, six valid zones, stable unique identifiers, valid routes, and no unresolved relationships.
- Content contract tests will require the exact 15-term foundations sequence and verify that every referenced prerequisite and next step exists.
- Content contract tests will verify that all lessons contain required metadata, learning stages, at least one valid source, and a verification date.
- Content contract tests will require one valid quick-check for each mini-lesson and five valid questions for each flagship lesson. Every question must have a determinable correct outcome and explanatory feedback.
- Unit tests will cover mastery threshold behavior, viewed-versus-mastered transitions, progress schema migration/validation, export/import round trips, and rejection of incompatible or malformed progress data.
- Analytics tests will verify the documented event names and payload privacy boundary without calling the live analytics service.
- Build validation will include Astro type/content checks, linting, formatting checks, unit tests, a production build, and browser tests.
- Performance validation will inspect representative page bundles and Lighthouse results, with special attention to ensuring Three.js is absent from ordinary non-3D initial loads.
- This is a greenfield workspace with no prior application test suite. The project therefore has no codebase test precedent to copy; the approved browser and content-contract seams establish the initial precedent.

## Out of Scope

- Copying or closely adapting prose, examples, or editorial arrangement from Matt Pocock's unlicensed source repository.
- User accounts, authentication, cloud-synchronized progress, social profiles, leaderboards, or cross-user features.
- Runtime AI-generated lessons, quizzes, grading, explanations, or a hosted AI tutor.
- Bring-your-own-model-key functionality.
- A hosted CMS or nontechnical publishing workflow.
- Automatic synchronization with the source dictionary.
- More than the agreed 71 initial concepts during the first release.
- A bespoke WebGL scene for every lesson or a true 3D global relationship graph.
- Unrestricted 3D sandbox controls.
- A full offline/PWA implementation or service worker.
- Native mobile applications.
- Legacy browser support outside the agreed modern evergreen range.
- Advanced gamification such as points, streaks, achievements, competition, or notifications.
- Adaptive quiz generation or personalized algorithmic learning paths.
- Comments, discussion forums, cohorts, instructor dashboards, or classroom management.
- A custom domain purchase or DNS migration.
- Publishing to Cloudflare before explicit authorization is obtained.
- Creating or connecting a GitHub remote as part of the site implementation.
- A guarantee of comprehensive bespoke screen-reader narration for every spatial detail beyond the required textual equivalents and launch accessibility safeguards.

## Further Notes

- Research found 71 terms in the source repository across seven source sections. The repository did not expose a content license at the inspected revision, so public visibility and attribution must not be treated as permission to copy or adapt its prose.
- The product's six-zone taxonomy and all educational writing are original project decisions. Factual term names may overlap with industry vocabulary and the research source.
- “Flagship” identifies lesson depth, not access level. Every concept ships with a useful lesson and assessment, and no lesson is locked.
- “2.5D atlas” means a readable two-dimensional relationship layout enhanced with scale, layering, shadows, animated paths, and focus transitions; it does not mean perspective navigation through an unlabeled 3D cloud.
- “Equivalent 2D fallback” means preserving the instructional states and explanation, not merely showing a decorative screenshot.
- The placeholder canonical URL must be replaced before public indexing is enabled on the final production domain.
- The tracker conventions require this specification to be published as a GitHub issue with the `ready-for-agent` label. The current workspace is not a Git repository and has no configured remote, so a target GitHub repository cannot currently be inferred for publication.
