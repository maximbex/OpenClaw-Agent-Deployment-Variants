# OpenClaw-Agent-Deployment-Variants

# **The Composable Agent Stack**

# **(For a personal reference architecture)**

### **A Dimensional Taxonomy & Validated Configurations**

To engineer a highly specific OpenClaw deployment, we must map the atomic variables (The Dimensions) and observe how they combine into viable, real-world ecosystems (The Validated Stacks). This framework serves as a definitive, 12-dimensional specification for distributed, local-first cognition, preserved under strict lossless architectural fidelity.

## **Part I: The Atomic Dimensions**

### **Dimension 1: The Substrate (Hardware, Location & Power Profile)**

*Where do the electrons flow, and at what thermal cost?*

1. **High-Memory Local (15W-40W):** Mac Mini M4 (16GB unified memory). *Power-Resilient Profile: Wake-on-LAN (WoL) summoned.*  
2. **Windows Workstation (100W+):** PC running Windows Subsystem for Linux (WSL2).  
3. **Persistent Home-Lab (15W-30W):** NAS (Synology, TrueNAS, Unraid, QNAP).  
4. **The Edge Node (\<5W):** Raspberry Pi 4/5, Orange Pi, Rock Pi. *Power-Resilient Profile: PoE HAT \+ UPS Battery Bank.*  
5. **Repurposed Hardware (20W-80W):** Spare desktop, tower, or the *Lid-Closed Dock-Station* (old laptop as headless node).  
6. **GPU Edge Node (10W-25W):** Hardware-accelerated edge devices (NVIDIA Jetson Nano/Orin).  
7. **Cloud Virtual Server:** Rented VPS (Hostinger, Hetzner, OVHcloud, Fly.io, DigitalOcean, Linode, AWS Lightsail, Contabo, GCP e2-micro).  
8. **High-Memory Cloud (Free Tier):** Oracle Cloud Always-Free (4 ARM CPUs \+ 24GB RAM).  
9. **Dedicated Agent Platforms / PaaS:** Specialized provisioners (ClawHost, Elest.io, Coolify).  
10. **Cloud GPU Marketplace / Serverless GPU:** Ephemeral, high-compute (RunPod, Vast.ai, Modal).  
11. **Cloud IDE Environments:** Browser-accessible workspaces (GitHub Codespaces, Gitpod).  
12. **Ultra-Mobile (Sandboxed) (\<5W):** Standard Android device (non-rooted Termux).  
13. **Rooted Mobile Sentinel (\<5W):** Smartphone as bare-metal ARM server with a built-in UPS.  
14. **Dedicated Mini PC (10W-65W):** Intel/AMD NUC, Beelink, or refurbished Thin Clients (HP/Dell Wyse).  
15. **Container PaaS / Serverless / Edge:** Managed runtimes (Railway, Render, Cloudflare Workers, Hugging Face Spaces).  
16. **iOS Local Node (\<5W):** iPhone/iPad running iSH or a-Shell \+ local Ollama.  
17. **Nomadic Network Hardware (\<5W):** Travel routers (GL.iNet) or Carputer/Vehicle setups.

### **Dimension 2: The Isolation Boundary (Security & Virtualization)**

*How is the blast radius contained?*

1. **Bare-Metal (Zero Isolation):** Running directly on the host OS.  
2. **User-Space Sandboxing:**   
   1. Firejail  
   2. [Bubblewrap](https://github.com/containers/bubblewrap)  
   3. [Bubblejail](https://github.com/igo95862/bubblejail)  
   4. [Systemd](https://www.reddit.com/r/linux/comments/knjzf2/comment/ghll5vm/?utm_source=share&utm_medium=web3x&utm_name=web3xcss&utm_term=1&utm_content=share_button)  
3. **Sandboxed Containerization:**   
   1. Docker natively on macOS/NAS with restricted templates  
   2. OrbStack   
4. **Lightweight Linux Containers:** LXC / LXD.  
5. **Rootless Containerization:**   
   1. Podman  
   2. Termux  
   3. iSH  
   4. a-Shell.  
6. **Hardware Virtualization:**   
   1. Dedicated VM  
      1. UTM   
      2. Parallels  
      3. VirtualBox  
   2. Type-1 Hypervisors   
      1. Proxmox VE  
7. **Cloud Micro-VMs:** Purpose-built, ephemeral sandboxes (E2B.dev).  
8. **Orchestrated Clusters:**   
   1. Kubernetes  
   2. Docker Swarm  
   3. K3s  
9. **Kernel-Level Policy:** Enterprise vaults  
   1. NemoClaw  
   2. OpenShell

### **Dimension 3: The Agentic Core (The Orchestrator)**

*What software framework manages the prompt loops?*

1. **OpenClaw (Canonical 2026):** The primary, highly-extensible framework.  
2. **Autonomous Software Engineers:**  
   1. OpenHands  
   2. Claude Code  
3. **Integrated IDE Agents:** Deep editor-tree integration  
   1. Cursor  
   2. Windsurf  
2. **Generic Consumer UI Wrappers:** Managed web interfaces  
   1. Claude.ai  
   2. Poe  
   3. HuggingChat  
   4. Kimi.com / bot UI  
2. **OS-Native & Desktop Wrappers:**  
   1. AnyClaw  
   2. Vellum  
   3. Claude Cowork  
2. **Design-Specific Claw Forks:**  
   1. NanoClaw  
   2. ZeroClaw  
   3. ZeptoClaw  
   4. Goclaw  
   5. safeclaw (LLM-less safety)  
2. **Hybrid Orchestrators:** The openclaw-n8n-stack or n8n standalone.  
3. **Multi-Instance Swarm (Single Host):** Parallel Claws via message queues (Redis).  
4. **Custom Production Frameworks:**  
   1. LangGraph  
   2. Microsoft AutoGen  
   3. CrewAI  
   4. Hermes Agent  
   5. Superagent  
2. **Visual Node Builders:**  
   1. Flowise  
   2. Langflow  
   3. Zapier Central

### **Dimension 4: The Cognitive Engine (Inference & Routing)**

*Where is the reasoning computed?*

2. **Frontier Cloud API:** Direct calls to  
   1. Claude Opus  
   2. Gemini Pro  
   3. OpenAI  
   4. Kimi  
   5. Qwen  
   6. Z.ai  
2. **Serverless & Managed Model Endpoints:** Open-weight models on shared hardware (Groq, Together AI) or custom weights on managed endpoints (Baseten, Modal).  
3. **Multi-Model Aggregators:** Dynamic routing (OpenRouter).  
4. **Free-Tier Extraction:**  
   1. Antigravity/Gemini CLI plugins  
   2. Hugging Face Inference API  
2. **Cloud-Hosted Open Weights:** Renting raw GPU to host a private model.  
   1. RunPod  
   2. Vast.ai  
2. **Pure Local Inference:**  
   1. Ollama  
   2. LM Studio  
   3. LocalAI  
   4. raw llama.cpp  
2. **The Tiered Router:** Local model triage; escalating for complexity.

### **Dimension 5: The Economic Stratum (Cost Model)**

*How is the cognitive engine sustained over time?*

1. **Absolute Zero:** Local hardware inference. (Electricity cost tracking acts as the sole underlying metric).  
2. **Load-Balanced Free Tiers:** API key rotation algorithms.  
3. **Fractional Utility (Pay-Per-Token):** Usage-based serverless or managed endpoints.  
4. **Pre-Bought Compute:** Episodic high-compute bursts (RunPod credits).  
5. **Subscription Caps:** Fixed monthly overhead (Claude Pro, Kimi+).

### **Dimension 6: Persistence (Memory & Sync Strategy)**

*How does the agent recall the past?*

1. **Stateless Worker:** Wiped clean after every task.  
2. **Ephemeral Cache:** Redis context.  
3. **Markdown Filesystem:** Flat-file text logs (SOUL.md).  
4. **Structured Datastore:**  
   1. SQLite  
   2. PostgreSQL  
5. **Git-Backed Memory:** Version-controlled state with audit trails.  
6. **Vector/RAG Database:** Semantic search.  
7. **Layered Stack:**  
   1. Redis (Short) \+ Markdown (Medium) \+ Vector (Long)  
2. **Federated Sync:** Master-Slave or Active-Active CRDTs (Syncthing).

### **Dimension 7: Network & Ingress (Transport Channels)**

*How does data traverse the perimeter?*

1. **Air-Gapped / Localhost-Only:** Bound to 127.0.0.1.  
2. **Mesh VPN & Tunnels:**  
   1. Tailscale  
   2. ZeroTier  
   3. Cloudflare Tunnel  
3. **Event-Driven Webhooks:** Generic HTTP callbacks.  
4. **Time-Based Interrogation:** Cron jobs fetching data.

### **Dimension 8: Interaction Surfaces (The Human Modalities)**

*What is the sensory modality with the operator?*

1. **The CLI Terminal:** Active IDE triggering.  
2. **The Omnichannel Bridge:**  
   1. Telegram  
   2. Discord  
   3. Matrix  
   4. WhatsApp  
   5. Slack  
   6. Signal  
3. **Universal Comm Triggers:**  
   1. Email (IMAP/SMTP).  
2. **Schedule Actuation:**  
   1. CalDAV calendar triggers.  
2. **Voice Invocation:**  
   1. Siri / Alexa shortcuts  
2. **IoT & Smart Home:**  
   1. Home Assistant API bindings

### **Dimension 9: Operational Role & Privilege (The Functional Ceiling)**

*What is the agent structurally permitted to execute?*

2. **The Full Orchestrator:** Holds state, UI, tools, and workflows.  
3. **The Gateway / Router Only:** Traffic forwarding to hidden backends.  
4. **The Inference Backend:** Dedicated model runner, no UI/logic.  
5. **The Automation Worker:** Headless node for background tasks.  
6. **The Ephemeral Canary:** Disposable test instance for validation.  
7. **Capability Limits:** Analyst-Only, Write-Limited, Sandboxed, or Unrestricted.

### **Dimension 10: Observability & Validation**

*How do we verify the daemon is breathing?*

1. **Passive Logging:** Manual tailing of logs.  
2. **Health Endpoints:** Exposing /health for JSON status.  
3. **Self-Hosted Dashboards:** Uptime Kuma monitoring.  
4. **Active Push Alerting:** Pushover or ntfy.  
5. **Status Bots:** Latency-reporting sub-bots.  
6. **Synthetic Polling:** Prompt-response verification.

### **Dimension 11: Continuity Mechanics**

*How does the agent survive failure?*

1. **Manual Restart:** Operator intervention.  
2. **Container-Native Resiliency:** Docker restart policies.  
3. **Healthcheck Auto-Restart:** Forceful reboot on unresponsiveness.  
4. **OS-Level Watchdog:** systemd persistence.  
5. **Battery/UPS Monitoring:** Graceful shutdown on low voltage.  
6. **Self-Healing Scripts:** pre-boot MEMORY.md syntax repair.  
7. **Hardware Wake States:** Wake-on-LAN (WoL).

### **Dimension 12: Replicability Strategy**

*How easily can this node be cloned?*

1. **Artisanal:** Manual, high friction.  
2. **Pre-Baked Images:** Packer VM artifacts.  
3. **Scripted:** docker-compose.yml.  
4. **Declarative State:** Nix / NixOS immutable configs.  
5. **Orchestrated:** Ansible playbooks.  
6. **GitOps:** Flux / ArgoCD.

## **Part II: Validated Configurations (The Matrix Model)**

| Archetype | Substrate/Isol. | Core/Engine | Mem./Role | Net./Interface | Ops |
| :---- | :---- | :---- | :---- | :---- | :---- |
| **The Sovereign Coder** | Mac M4 (VM) | OpenClaw / Tiered | Git-Backed / Full Orch. | Air-Gapped / CLI | WoL / NixOS |
| **The Disposable Scout** | Cloud IDE (B7) | OpenHands / Managed | Stateless / Canary | Mesh VPN / CLI | Scripted |
| **The Neo-Village Fed.** | Mac+NAS+Pi (Docker) | OpenClaw / Tiered | CRDT Sync / Full Orch. | Mesh VPN / Omnichannel | systemd / Ansible |
| **The Oracle Anchor** | Oracle (24GB) / LXC | OpenClaw / Serverless | SQLite / Persistent | Mesh VPN / Webhooks | systemd / Syncthing |
| **The Cybernetic Lab** | Repurposed HW (Podman) | Multi-Instance / Bypass | Markdown / Automation | Localhost / Cron | Healthcheck / Compose |
| **The Persistent Daemon** | Synology NAS (Sandbox) | OpenClaw / Bypass | SQLite / Full Orch. | Mesh VPN / Telegram | Auto-Restart / Compose |
| **The Load-Balanced Edge** | Oracle \+ VPS (LXC) | OpenClaw / Key Rot. | Redis / Gateway Only | Webhooks / WhatsApp | Healthcheck / Ansible |
| **The Voice-First Sentinel** | iPad (Rootless) | AnyClaw / Pure Local | Markdown / Full Orch. | Localhost / Siri | Battery Mon. / Artisanal |
| **The Stealth Node** | Router (Firejail) | BabyClaw / Serverless | Stateless / Canary | Mesh VPN / Slack | Watchdog / Scripted |
| **The Nomadic Node** | Travel Router (Docker) | OpenClaw / Serverless | Markdown / Gateway | ZeroTier / Email | Battery Mon. / Scripted |
| **The Rooted Sentinel** | Pixel 5 (Linux Deploy) | OpenClaw / Serverless | Markdown / Full Orch. | Mesh VPN / Voice | Battery Mon. / Artisanal |
| **The GitOps Backend** | Cloud VPS (K8s) | OpenClaw / Serverless | Vector / Backend Only | Webhooks / None | K8s Probes / Flux |
| **The Architect's Blueprint** | Mac M4 (Rootless) | Obsidian / Anthropic | Git-Backed / Read-Only | Air-Gapped / CLI | Manual / Ansible |

## **Part III: The Discarded Topologies (Explicit Rejections)**

* **Generic Corporate Nomenclature (e.g., "Local single-user desktop")**  
  * *Reason:* **Aesthetic Atrophy.** Dull nomenclature is rejected while preserving the underlying topologies.  
* **The Managed Premium (OpenClaw Cloud / KiloClaw / OneClaw / MyClaw / Duet)**  
  * *Reason:* **Epistemic Surrender.** Outsourcing core infrastructure strips filesystem sovereignty.  
* **The Consumer Chat Interface (Kimi.com UI / Poe / Claude.ai)**  
  * *Reason:* **Interaction-Only Constraint.** While useful for prompt-testing (**The Canary Test Harness**), these remain discarded as *Primary Persistent Daemons* due to a lack of mechanical agency over the local filesystem. This rejection applies specifically to the **UI wrapper**, not the underlying cognitive API models.  
* **The Permanent Cloud Forge (RunPod / Vast.ai)**  
  * *Reason:* **State Loss & Hemorrhage.** GPUs are for *episodic* heavy lifting, not continuous residence.  
* **The Desktop Automator (Claude Cowork / Vellum)**  
  * *Reason:* **Headless Incompatibility.** These tools brilliantly automate active macOS desktop sessions but fail as headless 24/7 background daemons due to GUI requirements.  
* **The Serverless Edge Phantom (Cloudflare Workers / AWS Fargate / Render)**  
  * *Reason:* **Impedance Mismatch.** Serverless PaaS architectures aggressively spin down idle containers, suffocating 24/7 WebSocket persistence.  
  * ***The Cron Exception:*** Viable *only* if the agent acts as a stateless automation worker mounting an external volume.  
* **The Browser Workspaces (GitHub Codespaces / Gitpod)**  
  * *Reason:* **Session Decay / Persistence Failure.** Discarded for the *Persistent Daemon* role.  
  * ***The Episodic Exception:*** These remain highly validated for **The Disposable Scout**, where decay is a security feature rather than a bug.  
* **The eGPU Tower (High-End PC \+ eGPU)**  
  * *Reason:* **Hardware Dissonance.** The M4's unified memory defines the ecosystem's elegance.  
* **The Fragile Puppeteer (baremobile / appclaw)**  
  * *Reason:* **Actuation Fragility.** Visual screen-puppeteering is unstable. We rely on API gateways.  
* **The Enterprise Swarm (Kubernetes \+ AutoGen/LangGraph)**  
  * *Reason:* **DevOps Asphyxiation.** Excessive maintenance burden for a single operator.

**Note**: This document is intended to be exhaustive / complete. If you find missing entries. Please let me know\!  
