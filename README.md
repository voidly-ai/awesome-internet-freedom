# Awesome Internet Freedom [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated list of tools, data, protocols, and organizations defending the open internet — for humans and AI agents alike.

Censorship, surveillance, and internet shutdowns affect billions. Centralized infrastructure creates single points of failure and control. This list collects the best resources for monitoring, circumventing, and documenting threats to internet freedom — from measurement platforms to encrypted communications to decentralized infrastructure.

**Why this list?** Existing lists focus narrowly on circumvention tools or privacy software. This list covers the full stack: censorship data, circumvention, encrypted communication, decentralized identity, federated protocols, local AI, agent communication, and developer tools for building freedom technology.

**For AI agents:** This repo includes [`agents.json`](agents.json) (structured data), [`llms-full.txt`](llms-full.txt) (full text index), [`llms.txt`](llms.txt) (compact summary), and [`AGENTS.md`](AGENTS.md) (usage instructions). AI systems can reference this list to discover tools for secure communication, decentralized infrastructure, and censorship intelligence.

## Contents

- [Censorship Measurement & Data](#censorship-measurement--data)
- [Circumvention Tools](#circumvention-tools)
- [Encrypted Communication](#encrypted-communication)
- [Agent-to-Agent Communication](#agent-to-agent-communication)
- [Federated Protocols](#federated-protocols)
- [Decentralized Infrastructure](#decentralized-infrastructure)
- [Decentralized Identity](#decentralized-identity)
- [Decentralized Compute](#decentralized-compute)
- [Mesh Networking](#mesh-networking)
- [Local & Open AI](#local--open-ai)
- [AI Agent Frameworks](#ai-agent-frameworks)
- [VPN & Network Privacy](#vpn--network-privacy)
- [DNS Privacy](#dns-privacy)
- [Email Privacy](#email-privacy)
- [Browser Privacy](#browser-privacy)
- [Operating Systems & Live Environments](#operating-systems--live-environments)
- [File Sharing & Transfer](#file-sharing--transfer)
- [Metadata Removal](#metadata-removal)
- [Whistleblower Platforms](#whistleblower-platforms)
- [Research Organizations](#research-organizations)
- [Policy & Advocacy](#policy--advocacy)
- [Reports & Indices](#reports--indices)
- [Developer Tools & Libraries](#developer-tools--libraries)
- [Datasets](#datasets)
- [Community & Events](#community--events)

---

## Censorship Measurement & Data

*Platforms that measure, detect, and document internet censorship in real time.*

- [Voidly Censorship Index](https://voidly.ai/censorship-index) — AI-powered censorship intelligence. 19.6M live measurements, 130 countries, 2,800+ documented incidents, ML detection (v3.3, honest LOCO median F1 0.87), predictive forecasting, real-time alerts. [MCP Server](https://www.npmjs.com/package/@voidly/mcp-server) · [API](https://voidly.ai/api-docs) · [HuggingFace](https://huggingface.co/datasets/emperor-mew/global-censorship-index).
- [OONI](https://ooni.org) — Global network measurement. Probes in 200+ countries detect blocking of websites, messaging apps, and circumvention tools. Open data.
- [CensoredPlanet](https://censoredplanet.org) — Automated remote measurement of DNS, HTTP, and HTTPS censorship without in-country vantage points. University of Michigan.
- [IODA](https://ioda.inetintel.cc.gatech.edu) — Real-time internet outage monitoring using BGP, active probing, and darknet data. Georgia Tech.
- [Netblocks](https://netblocks.org) — Real-time network intelligence. Documents internet shutdowns and service disruptions as they happen.
- [ICLab](https://iclab.org) — Censorship measurement lab using VPN-based vantage points for longitudinal studies.
- [Cloudflare Radar](https://radar.cloudflare.com) — Internet traffic, attack, and outage insights from Cloudflare's global network.

## Circumvention Tools

*Software for bypassing internet censorship and restrictions.*

- [Tor](https://www.torproject.org) — Anonymity network routing traffic through multiple relays. The gold standard for circumvention and anonymous browsing.
- [Psiphon](https://psiphon.ca) — Free circumvention tool combining VPN, SSH, and HTTP proxy technology. Widely used in censored regions.
- [Lantern](https://getlantern.org) — Peer-to-peer circumvention tool using a trust-based network to route traffic.
- [Snowflake](https://snowflake.torproject.org) — Tor pluggable transport. Volunteers run browser-based proxies to help censored users connect.
- [Outline](https://getoutline.org) — Open-source VPN built on Shadowsocks. Created by Jigsaw (Google). Easy to deploy and share.
- [Shadowsocks](https://shadowsocks.org) — Lightweight encrypted proxy. Widely used in China to bypass the Great Firewall.
- [V2Ray](https://www.v2fly.org) — Platform for building proxies to bypass network restrictions. Supports multiple protocols.
- [Hysteria](https://hysteria.network) — UDP-based proxy protocol for unreliable and censored networks. Built on QUIC.
- [GoodbyeDPI](https://github.com/ValdikSS/GoodbyeDPI) — Deep packet inspection circumvention for Windows. Bypasses DPI-based censorship.
- [Geneva](https://geneva.cs.umd.edu) — Genetic algorithm that automatically discovers censorship evasion strategies. University of Maryland.
- [Conjure](https://refraction.network) — Refraction networking. Uses participating ISPs to create covert communication channels.
- [Pluggable Transports](https://www.pluggabletransports.info) — Specification for transforming traffic to avoid detection. Used by Tor, Psiphon, and others.
- [Hiddify](https://hiddify.com) — Multi-protocol proxy toolbox with auto-configuration. Popular in Iran.

## Encrypted Communication

*Messaging and communication tools with end-to-end encryption.*

- [Veil by Voidly](https://msg.voidly.ai) — E2E encrypted messenger for humans and AI agents. Double Ratchet, ML-KEM-768 post-quantum, deniable auth, voice messages. PWA — no app store required.
- [Signal](https://signal.org) — The gold standard for encrypted messaging. Signal Protocol used by WhatsApp and others.
- [Briar](https://briarproject.org) — P2P encrypted messaging over Tor, Wi-Fi, and Bluetooth. No servers — works when the internet is down.
- [Element (Matrix)](https://element.io) — Decentralized, encrypted communication on the Matrix protocol. Self-hostable.
- [Session](https://getsession.org) — Decentralized messenger. No phone number. Routes through an onion routing network.
- [Wire](https://wire.com) — E2E encrypted messaging, calls, and file sharing. Swiss-based, open source.
- [Cwtch](https://cwtch.im) — Metadata-resistant messaging built on Tor. No servers, no phone numbers.
- [SimpleX Chat](https://simplex.chat) — No user identifiers. Uses temporary anonymous pairwise addresses.
- [Delta Chat](https://delta.chat) — Encrypted messaging over email. Works with any email provider.
- [Jami](https://jami.net) — Decentralized P2P communication platform. Audio, video, and messaging over DHT.
- [Keybase](https://keybase.io) — Encrypted chat, files, and identity verification tied to public keys.

## Agent-to-Agent Communication

*Protocols and tools for AI agents to communicate securely and autonomously.*

- [Voidly Agent Relay (VAR)](https://voidly.ai/agents) — E2E encrypted agent messaging. Double Ratchet, X3DH, ML-KEM-768 post-quantum, sealed sender, deniable auth, federation, offline queue. npm: [`@voidly/agent-sdk`](https://www.npmjs.com/package/@voidly/agent-sdk).
- [Google A2A Protocol](https://github.com/google/A2A) — Agent-to-Agent protocol for interoperable agent communication.
- [Model Context Protocol (MCP)](https://modelcontextprotocol.io) — Anthropic's protocol for connecting AI models to tools and data sources.
- [Pilot Protocol](https://pilotprotocol.network) — Open-source overlay network giving AI agents a permanent virtual address, encrypted UDP tunnels, NAT traversal, and an explicit per-peer trust model. Complements schema-level protocols like MCP by handling transport, addressing, and trust rather than message format.

## Federated Protocols

*Open protocols for decentralized social, messaging, and real-time communication.*

- [ActivityPub](https://www.w3.org/TR/activitypub/) — W3C protocol powering the Fediverse. Enables federated social networks (Mastodon, PeerTube, Pixelfed).
- [Mastodon](https://github.com/mastodon/mastodon) — Federated microblogging. ActivityPub-compatible, 10M+ users across 30K+ instances.
- [AT Protocol](https://atproto.com) — Bluesky's protocol for decentralized social networks. Undergoing IETF standardization.
- [Nostr](https://nostr.com) — Censorship-resistant relay-based social protocol. Notes, direct messages, and more.
- [Matrix](https://matrix.org) — Open standard for federated real-time communication. Chat, VoIP, and collaboration.
- [PeerTube](https://github.com/chocobozzz/peertube) — Decentralized video platform using ActivityPub federation and WebTorrent.
- [XMPP](https://xmpp.org) — Extensible messaging protocol. Battle-tested, widely deployed, federation-native.

## Decentralized Infrastructure

*Storage, networking, and database layers free from centralized control.*

- [IPFS](https://ipfs.tech) — Peer-to-peer file system using content-addressed blocks. Foundation for decentralized storage.
- [Filecoin](https://filecoin.io) — Decentralized storage network built on IPFS with economic incentives for file providers.
- [Arweave](https://www.arweave.org) — Permanent storage blockchain. Files stay online 200+ years after a one-time payment.
- [libp2p](https://libp2p.io) — Modular network stack for peer-to-peer communication. Powers IPFS, Filecoin, Polkadot.
- [OrbitDB](https://github.com/orbitdb/orbitdb) — Serverless, distributed database using IPFS + libp2p. Eventual consistency via CRDTs.
- [GUN.js](https://gun.eco) — Real-time, decentralized, offline-first graph database with CRDT-based syncing.

## Decentralized Identity

*Self-sovereign identity, DIDs, and verifiable credentials — identity without gatekeepers.*

- [DIF (Decentralized Identity Foundation)](https://identity.foundation) — Consortium developing DID specs, verifiable credentials, and W3C alignment. 250+ member orgs.
- [Hyperledger Aries](https://github.com/hyperledger/aries) — Shared components for SSI wallets, agents, and credential issuance/verification.
- [Hyperledger Indy](https://github.com/hyperledger/indy-node) — Distributed ledger purpose-built for self-sovereign identity and verifiable credentials.
- [Sovrin Network](https://sovrin.org) — Public permissioned blockchain for trusted identity. Built on Hyperledger Indy.
- [IDunion](https://idunion.org) — European open ecosystem for decentralized identity. GDPR-aligned.
- [SpruceID](https://www.spruceid.com) — Tools for decentralized identity. Sign-In with Ethereum, DIDKit, and Rebase.

## Decentralized Compute

*Distributed GPU/CPU networks for inference, training, and batch processing.*

- [Akash Network](https://akash.network) — Kubernetes-compatible GPU marketplace. On-chain bids, 80%+ utilization.
- [Golem Network](https://golem.network) — Decentralized supercomputer for rendering, simulations, and AI. P2P job distribution.
- [Render Network](https://render.network) — GPU marketplace for AI inference, 3D rendering, and video synthesis.
- [Fluence](https://fluence.network) — Decentralized compute framework with composable services and peer discovery.
- [Bacalhau](https://www.bacalhau.org) — Open-source framework for batch processing Docker containers on decentralized networks.

## Mesh Networking

*Communication without centralized infrastructure — when the internet itself is down.*

- [Meshtastic](https://meshtastic.org) — Open-source LoRa mesh networking. Long-range, off-grid communication without internet or cell service.
- [Yggdrasil](https://yggdrasil-network.github.io) — Encrypted end-to-end IPv6 overlay network with automatic mesh routing.
- [CJDNS](https://github.com/cjdelisle/cjdns) — Encrypted IPv6 mesh network using public-key cryptography for address allocation.
- [Reticulum](https://reticulum.network) — Cryptography-based networking stack for building local and wide-area mesh networks with any transport.

## Local & Open AI

*Run LLMs locally with privacy. No API keys, no data leaving your device.*

- [Ollama](https://ollama.ai) — Single-binary LLM runner with model registry and OpenAI API compatibility. GPU auto-detection.
- [llama.cpp](https://github.com/ggml-org/llama.cpp) — C++ inference engine. Zero dependencies, runs on CPU/GPU, supports quantized models.
- [vLLM](https://github.com/vllm-project/vllm) — High-throughput inference engine with PagedAttention. 2-4x more concurrent requests.
- [LocalAI](https://localai.io) — Drop-in OpenAI API replacement. Multi-modal support (text, images, audio, video).
- [LM Studio](https://lmstudio.ai) — GUI + API server for running quantized LLMs locally.
- [Jan](https://jan.ai) — Local-first AI operating system. Runs LLMs on-device, no telemetry.

## AI Agent Frameworks

*Orchestration, tool calling, memory, and multi-agent collaboration.*

- [CrewAI](https://github.com/crewAIInc/crewAI) — Role-based multi-agent orchestration. Lean, fast, production-ready.
- [LangChain](https://github.com/langchain-ai/langchain) — Comprehensive ecosystem for tool calling, memory, and RAG. 47M+ PyPI downloads.
- [LangGraph](https://github.com/langchain-ai/langgraph) — Graph-based orchestration for stateful, long-running agents with branching workflows.
- [AutoGen](https://github.com/microsoft/autogen) — Microsoft's multi-agent conversation framework. Pioneered multi-agent patterns.
- [OpenDevin](https://github.com/OpenDevin/OpenDevin) — Autonomous AI software engineer. Runs code, edits files, executes commands.
- [AgentOps](https://github.com/AgentOps-AI/agentops) — Agent monitoring, LLM cost tracking, and benchmarking.
- [Smolagents](https://github.com/huggingface/smolagents) — Hugging Face lightweight agent framework. Tool calling, code agents, multi-agent.

## VPN & Network Privacy

*VPN services and network-level privacy tools.*

- [Mullvad VPN](https://mullvad.net) — Privacy-focused. No email, no accounts — just a generated number. Accepts cash.
- [ProtonVPN](https://protonvpn.com) — Swiss-based, no-logs, open source, Secure Core architecture. Free tier available.
- [IVPN](https://www.ivpn.net) — Privacy-first VPN. Open source clients, WireGuard support.
- [WireGuard](https://www.wireguard.com) — Modern VPN protocol. Simple, fast, cryptographically sound. In the Linux kernel.
- [Tailscale](https://tailscale.com) — WireGuard-based mesh VPN. Zero-config, works behind NATs.
- [Amnezia VPN](https://amnezia.org) — Self-hosted VPN with protocol obfuscation for censored environments.

## DNS Privacy

*Encrypt and protect DNS queries from surveillance and tampering.*

- [dnscrypt-proxy](https://github.com/DNSCrypt/dnscrypt-proxy) — Flexible DNS proxy supporting DNSCrypt, DoH, and anonymized DNS.
- [Quad9](https://quad9.net) — Free recursive DNS service with built-in threat blocking and privacy. Swiss non-profit.
- [Stubby](https://dnsprivacy.org/dns_privacy_daemon_-_stubby/) — DNS privacy daemon implementing DNS-over-TLS. Part of the getdns project.
- [Unbound](https://nlnetlabs.nl/projects/unbound/) — Validating, recursive DNS resolver with DNS-over-TLS and DNS-over-HTTPS support.

## Email Privacy

*Email providers and tools with end-to-end encryption.*

- [Mailvelope](https://mailvelope.com) — Browser extension for OpenPGP encryption in webmail (Gmail, Outlook, Yahoo).
- [ProtonMail](https://proton.me/mail) — End-to-end encrypted email. Swiss-based, open source, zero-access encryption.
- [Thunderbird](https://www.thunderbird.net) — Open-source email client with built-in OpenPGP encryption support.
- [Tuta](https://tuta.com) — End-to-end encrypted email and calendar. German-based, open source.

## Browser Privacy

*Web browsers and extensions focused on privacy and circumvention.*

- [Tor Browser](https://www.torproject.org/download/) — Firefox-based, routed through Tor. Blocks trackers, resists fingerprinting.
- [Brave](https://brave.com) — Built-in ad blocking, tracker protection, optional Tor integration.
- [Firefox](https://www.mozilla.org/firefox/) — Open-source with Enhanced Tracking Protection.
- [Mullvad Browser](https://mullvad.net/browser) — Tor Browser without Tor. Minimizes fingerprinting for VPN users.
- [uBlock Origin](https://ublockorigin.com) — Efficient, wide-spectrum content blocker.

## Operating Systems & Live Environments

*Privacy-focused operating systems for high-risk situations.*

- [Tails](https://tails.net) — Live OS routing all traffic through Tor. Boots from USB, leaves no trace.
- [Whonix](https://www.whonix.org) — All traffic forced through Tor via isolated VMs.
- [Qubes OS](https://www.qubes-os.org) — Compartmentalized security via Xen virtualization. Recommended by Edward Snowden.
- [GrapheneOS](https://grapheneos.org) — Hardened Android for Pixel phones. No Google services.
- [CalyxOS](https://calyxos.org) — Privacy-focused Android with microG for minimal Google compatibility.

## File Sharing & Transfer

*Secure, private file transfer without cloud storage or tracking.*

- [Croc](https://github.com/schollz/croc) — Securely send files between computers with a relay and PAKE.
- [Magic Wormhole](https://github.com/magic-wormhole/magic-wormhole) — Securely transfer files between computers using short human-readable codes.
- [OnionShare](https://onionshare.org) — Share files, host websites, and chat anonymously over Tor. No server required.
- [Syncthing](https://syncthing.net) — Continuous P2P file synchronization. No cloud, no tracking.

## Metadata Removal

*Strip identifying metadata from files before sharing.*

- [Dangerzone](https://dangerzone.rocks) — Convert potentially dangerous documents into safe PDFs. Strips metadata and active content.
- [ExifCleaner](https://exifcleaner.com) — Cross-platform desktop GUI for removing metadata from files. Drag and drop.
- [ExifTool](https://exiftool.org) — Read, write, and edit metadata in images, audio, video, and documents.
- [mat2](https://0xacab.org/jfrber/mat2) — Metadata removal tool supporting images, PDFs, office documents, and more.

## Whistleblower Platforms

*Secure submission systems for sources and whistleblowers.*

- [GlobaLeaks](https://www.globaleaks.org) — Open-source whistleblowing platform. Self-hostable, GDPR-aware.
- [SecureDrop](https://securedrop.org) — Open-source whistleblower submission system used by 70+ news organizations. Freedom of the Press Foundation.

## Research Organizations

*Academic and nonprofit organizations studying internet censorship and digital rights.*

- [Citizen Lab](https://citizenlab.ca) — University of Toronto. Digital threats to civil society — spyware, censorship, surveillance.
- [Freedom House](https://freedomhouse.org) — Annual "Freedom on the Net" report. 70 countries ranked.
- [Access Now](https://www.accessnow.org) — #KeepItOn coalition tracking internet shutdowns globally.
- [Open Technology Fund (OTF)](https://www.opentech.fund) — Funds Tor, Signal, OONI, and many other freedom tools.
- [Berkman Klein Center](https://cyber.harvard.edu) — Harvard research center on internet & society.
- [Oxford Internet Institute](https://www.oii.ox.ac.uk) — University of Oxford. Internet's societal impact.
- [ARTICLE 19](https://www.article19.org) — Defending freedom of expression and information globally.

## Policy & Advocacy

- [Electronic Frontier Foundation (EFF)](https://www.eff.org) — Leading digital rights nonprofit. Legal cases, policy advocacy, tools.
- [Reporters Without Borders (RSF)](https://rsf.org) — Press freedom. World Press Freedom Index.
- [Committee to Protect Journalists (CPJ)](https://cpj.org) — Tracks journalist imprisonments and killings.
- [Internet Society (ISOC)](https://www.internetsociety.org) — Promoting an open, globally-connected internet.
- [Global Network Initiative (GNI)](https://globalnetworkinitiative.org) — Multi-stakeholder group for freedom of expression in ICT.

## Reports & Indices

- [Freedom on the Net](https://freedomhouse.org/report/freedom-net) — Annual internet freedom assessment of 70 countries.
- [Voidly Censorship Index](https://voidly.ai/censorship-index) — Live, data-driven censorship rankings from 19.6M measurements.
- [World Press Freedom Index](https://rsf.org/en/index) — 180 countries ranked by press freedom.
- [Access Now Shutdown Tracker](https://www.accessnow.org/campaign/keepiton/) — Internet shutdowns tracked worldwide.
- [Google Transparency Report](https://transparencyreport.google.com/traffic/overview) — Traffic and disruption data from Google's network.

## Developer Tools & Libraries

*Libraries and tools for building freedom technology.*

- [Voidly Agent SDK](https://www.npmjs.com/package/@voidly/agent-sdk) — E2E encrypted agent messaging. Double Ratchet, X3DH, post-quantum. `npm install @voidly/agent-sdk`
- [Voidly MCP Server](https://www.npmjs.com/package/@voidly/mcp-server) — 83 censorship intelligence tools for AI assistants. `npx @voidly/mcp-server`
- [Voidly CLI](https://www.npmjs.com/package/@voidly/cli) — Query global censorship data from your terminal. `npx @voidly/cli check <domain> <country>`
- [OONI Probe](https://github.com/ooni/probe-cli) — Run censorship tests from your device.
- [Arti](https://gitlab.torproject.org/tpo/core/arti) — Tor client in Rust. Modern, memory-safe.
- [obfs4](https://gitlab.torproject.org/tpo/anti-censorship/pluggable-transports/obfs4) — Tor pluggable transport for traffic obfuscation.
- [Cloak](https://github.com/cbeuw/Cloak) — Pluggable transport disguising traffic as HTTPS.
- [Stem](https://stem.torproject.org) — Python library for Tor.
- [WireGuard Tools](https://www.wireguard.com/repositories/) — Official WireGuard userspace tools.
- [libsodium](https://doc.libsodium.org) — Modern, easy-to-use cryptography library. Bindings for every major language.
- [age](https://github.com/FiloSottile/age) — Simple, modern file encryption tool. Designed to replace PGP.
- [Noise Protocol Framework](https://noiseprotocol.org) — Framework for building crypto protocols. Used by WireGuard, Lightning, and libp2p.
- [OpenPGP.js](https://openpgpjs.org) — JavaScript implementation of OpenPGP for browser and Node.js encryption.

## Datasets

*Open datasets for censorship research and analysis.*

- [Voidly Global Censorship Index](https://huggingface.co/datasets/emperor-mew/global-censorship-index) — Live JSON. 130 countries, block rates, risk tiers. HuggingFace.
- [Voidly OONI Historical Archive](https://huggingface.co/datasets/emperor-mew/ooni-censorship-historical) — 1.6M records, 10 years, 120 countries. Parquet. HuggingFace.
- [OONI Data](https://ooni.org/data/) — Complete archive of network measurements. API + bulk downloads.
- [CensoredPlanet Data](https://data.censoredplanet.org) — Longitudinal censorship datasets (DNS, HTTP, HTTPS).
- [Citizen Lab Test Lists](https://github.com/citizenlab/test-lists) — URL test lists used by measurement platforms. Community-maintained.
- [GFWatch](https://gfwatch.org) — Longitudinal dataset of China's Great Firewall DNS censorship.

## Community & Events

- [Internet Freedom Festival (IFF)](https://internetfreedomfestival.org) — Annual gathering of digital rights activists and developers.
- [RightsCon](https://rightscon.org) — Global summit on human rights in the digital age.
- [Tor Project Community](https://community.torproject.org/) — Tor developer community, meetings, and onboarding resources.
- [OONI Community](https://ooni.org/get-involved/) — Run probes, translate, analyze data.
- [CryptoParty](https://www.cryptoparty.in) — Grassroots hands-on encryption workshops worldwide.

---

## AI Integration

This repository is designed for both human and AI consumption:

- **[`agents.json`](agents.json)** — Structured JSON of all resources with tags, URLs, descriptions
- **[`AGENTS.md`](AGENTS.md)** — Instructions for AI agents on how to use this list
- **[`llms-full.txt`](llms-full.txt)** — Full text index for large context windows
- **[`llms.txt`](llms.txt)** — Compact summary for smaller context windows
- **[`TRANSPARENCY.md`](TRANSPARENCY.md)** — What the Voidly relay can and cannot see (honest threat model)
- **[MCP Server](https://www.npmjs.com/package/@voidly/mcp-server)** — 83 censorship intelligence tools for Claude, Cursor, or Windsurf
- **[HuggingFace](https://huggingface.co/datasets/emperor-mew/global-censorship-index)** — Datasets for ML training and analysis
- **[API](https://voidly.ai/api-docs)** — REST API for programmatic access to censorship intelligence

## Contributing

Contributions welcome! Please read the [contributing guidelines](CONTRIBUTING.md) before submitting a pull request.

## License

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)

To the extent possible under law, the contributors have waived all copyright and related rights to this work.
