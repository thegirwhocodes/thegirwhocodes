# Hi, I'm Naomi

**Computer Science & Economics at Wesleyan University · Founder of Sabi & Education for Equality.**  
Building voice-first AI systems, low-latency telephony agents, and real-time machine learning pipelines engineered under real-world infrastructure and bandwidth constraints.

---

### 🧰 What I use

**AI, Agents & Real-Time Voice**

[![AI & Machine Learning](https://skillicons.dev/icons?i=py,pytorch,fastapi,docker&perline=6)](https://skillicons.dev)  
`LangGraph` · `LangChain` · `OpenAI Realtime (WebSockets)` · `Google Gemini Live` · `Claude API` · `Whisper (LoRA)` · `ElevenLabs` · `MediaPipe`

**Full-Stack & Systems**

[![Web & Mobile](https://skillicons.dev/icons?i=ts,react,nextjs,nodejs,tailwind,swift&perline=6)](https://skillicons.dev)

**Data, Telephony & Cloud Infrastructure**

[![Data & Infrastructure](https://skillicons.dev/icons?i=postgres,supabase,linux,bash,c,cpp,git,gcp&perline=8)](https://skillicons.dev)  
`Asterisk PBX` · `SIP Trunking` · `G.711 μ-law Audio Codecs` · `Vultr Cloud (Johannesburg Edge)` · `RunPod Serverless GPU` · `Redis` · `Sentry`

---

### 🔒 Private Repositories & Access Request

> [!IMPORTANT]
> ### Reviewing My Production Codebase
> Most of my active production systems—including the **Sabi** phone telephony backend, custom Asterisk PBX routing, live Vultr Johannesburg containers, and LoRA training harnesses—live in private repositories for production security and company IP reasons.
>
> **Hiring managers, recruiters, and engineering teams:** If you would like collaborator read-access to audit the production Sabi codebase, Asterisk SIP pipelines, or evaluation suites, **[request private repo access here](mailto:nivie@wesleyan.edu?subject=Request%20Private%20Repository%20Access%20(Sabi)&body=Hi%20Naomi,%0D%0A%0D%0AI%20would%20like%20to%20review%20the%20Sabi%20production%20codebase%20and%20telephony%20pipelines.%0D%0A%0D%0AMy%20GitHub%20username%20is:%20%0D%0AOrganization%20/%20Role:%20%0D%0A%0D%0AThanks!)** or email me directly at **`nivie@wesleyan.edu`** with your GitHub handle. I am glad to grant immediate access.

---

### 📌 Featured Work

Most of what I build now lives in private startup and production systems. Below are key public repositories and architectural deep-dives:

**[Ayo / SafeLine](https://github.com/thegirwhocodes/safe-line)** *(HackPrinceton Fall '26 · LangChain, Healthcare & Sponsor Tracks)*  
*Full-duplex crisis telephony and silent-text triage platform with clinical trauma grounding and deterministic safety guardrails.*
* **Deterministic LangGraph Pipeline:** Architected a 4-node state machine (`pii_scrubber` → dual-engine risk scorer → trauma responder → automated caseworker dispatch) enforcing a hard regex safety floor alongside Gemini evaluation.
* **Low-Latency Telephony Audio Filter:** Wrote a pure-Python integer 3:1 decimation filter with precomputed lookup tables converting 24 kHz Gemini Live audio into 8 kHz G.711 $\mu$-law for telephony with sub-millisecond conversion and zero external C dependencies.
* **Voice Biometrics:** Spliced ReDimNet2+ speaker recognition models over 8 kHz audio channels, enabling zero-credential caller re-identification across anonymous and burner numbers.
* **Rigorous Synthetic Evals:** Engineered an automated 40-case synthetic evaluation suite across Nigerian Pidgin, British, and US vernacular—achieving **100.0% escalation recall** on crisis and **0.0% false positives**.

**[Sabi / Education for Equality](https://github.com/thegirwhocodes/sabi-server)** *(Flagship Venture · 501(c)(3) · [Request Private Access](mailto:nivie@wesleyan.edu?subject=Request%20Private%20Repository%20Access%20(Sabi)&body=Hi%20Naomi,%0D%0A%0D%0AI%20would%20like%20to%20review%20the%20Sabi%20production%20codebase%20and%20telephony%20pipelines.%0D%0A%0D%0AMy%20GitHub%20username%20is:%20%0D%0AOrganization%20/%20Role:%20%0D%0A%0D%0AThanks!))*  
*AI-powered voice tutor delivering foundational literacy and numeracy to 33M+ under-educated children across Nigeria over standard 2G telephony (`+234 201 700 1459`) at ~$0.41/student marginal cost.*
* **Full-Duplex Telephony Pipeline:** Streams bidirectional 8 kHz G.711 $\mu$-law audio via Africa's Talking SIP trunking into an Asterisk PBX and FastAPI WebSocket orchestrator connected to OpenAI Realtime (`gpt-realtime-2.1`) and ElevenLabs TTS.
* **Acoustic Adaptation & Fine-Tuning:** Fine-tuned Whisper STT with LoRA on RunPod GPUs ([thegirwhocodes/sabi-stt](https://github.com/thegirwhocodes/sabi-stt)) against AfriSpeech and Common Voice corpora, incorporating telephone-codec compression and ambient street noise augmentation to accurately transcribe accented Nigerian English.
* **Edge Deployment:** Deployed on dedicated Ubuntu nodes in Johannesburg (Vultr) to minimize intercontinental telephony round-trip latency to sub-800ms across West African cellular networks.
* **Recognition & Pilots:** Selected for the **UNICEF AI Ventures Accelerator** ($10,000 equity-free track) and active evaluation cohort with ~500 secondary school students in Rivers State.

**[Dactyl](https://github.com/thegirwhocodes/Dactyl-Final)** *(1st Place Overall Grand Champion · Morgan Hacks 2026)*  
*Bidirectional American Sign Language (ASL) smart glasses: real-time sign-to-speech and speech-to-AR captioning.*
* **Kinematic Tracking & Classification:** Extracted skeletal landmarks using MediaPipe feeding a hybrid Temporal Graph Convolutional Network (TGCN) + LSTM classifier to recognize continuous dynamic sign sequences.
* **Spatial Grammar Resolution:** Built a non-manual marker (NMM) facial expression detection pipeline and integrated Claude API context rewriting to resolve grammatical spatial ambiguity in ASL, delivering synthesized speech in <1.2 seconds.

**[Adjutant](https://github.com/thegirwhocodes/adjutant)** *(SCSP GenAI Hackathon · Team Charlie Mike · GenAI.mil Track)*  
*Completely air-gapped, offline voice assistant for tactical military documentation on isolated field hardware.*
* **Spoken-to-Schema Extraction:** Built multi-turn voice-to-JSON extraction mapping natural language requests directly to Department of the Army PDF forms (DA-31 Leave, DA-4856 Counseling, DD-1351-2 Travel with JTR per-diem math) with automatic regulatory citation validation in <15 seconds.

**[Sage Mail](https://github.com/thegirwhocodes/email)** *(Voice-First Gmail Agent)*  
*Voice-first email triage agent that prioritizes high-impact messages, drafts in the user's authentic tone, and strictly gates all sends behind human approval.* Next.js, Gmail OAuth, Claude, streaming voice UI.

**[Ed.it](https://github.com/thegirwhocodes/edit)** *(Desktop AI Video Editing Agent)*  
*Local desktop video editor driven by natural language.* Drop a raw clip, enter an edit brief, and an autonomous engine executes FFmpeg timeline cuts, audio leveling, and scene transitions via Claude Agent SDK and Gemini video understanding.

**[Go](https://github.com/thegirwhocodes/Go)** *(Commitment Device iOS Application)*  
*Native iOS application enforcing behavioral commitments through real financial stakes.* Integrates Apple CoreLocation geofencing and Google Calendar API to compute dynamic walking/transit ETAs, automatically triggering Stripe payment penalties when destination geofences are breached past scheduled start times.

---

### 🚧 Right Now

* **Scaling Sabi:** Preparing deployment pipelines and monitoring infrastructure for an active ~500-student school evaluation and Lagos pilot expansion.
* **Low-Latency Telephony Systems:** Hardening Asterisk SIP routing, G.711 $\mu$-law audio pipelines, and edge inference on Vultr Johannesburg nodes.
* **Undergraduate Studies:** Pursuing a B.A. in Computer Science & Economics at **Wesleyan University** (Class of 2027, 3.7 CGPA).

---

### 📊 GitHub Activity

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=thegirwhocodes&show_icons=true&theme=tokyonight&hide_border=true&bg_color=0D1117&count_private=true&include_all_commits=true" alt="Naomi's GitHub Stats" />
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=thegirwhocodes&layout=compact&theme=tokyonight&hide_border=true&bg_color=0D1117" alt="Top Languages" />
</p>

---

### 📫 Say Hi

I am interested in **Early-Career AI Systems, Deployed Engineering, and Founding Engineer roles** where agent reliability, evaluation rigor, and low-latency infrastructure matter.

* **Email:** [nivie@wesleyan.edu](mailto:nivie@wesleyan.edu)
* **LinkedIn:** [linkedin.com/in/naomi-ivie](https://linkedin.com/in/naomi-ivie)
* **Portfolio:** [naomiivie.vercel.app](https://naomiivie.vercel.app)
* **GitHub:** [@thegirwhocodes](https://github.com/thegirwhocodes)
