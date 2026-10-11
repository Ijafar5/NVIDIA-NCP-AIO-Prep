# NCP-AIO Daily Learning Roadmap

This is a **living plan**, not a fixed schedule. One "day" means one focused study session; if a lab takes multiple sessions, continue it rather than skipping ahead. Completion is based on demonstrated skill, not elapsed time.

## Exam alignment

The official professional exam blueprint groups skills into four domains:

| Domain | Published weighting |
| --- | ---: |
| Installation and Deployment | 31% |
| Administration | 23% |
| Workload Management | 23% |
| Troubleshooting and Optimization | 23% |

Source: [official NVIDIA NCP-AIO certification page](https://www.nvidia.com/en-us/learn/certification/ai-operations-professional/). Verify current objectives periodically. The prerequisite days below support the practical domains; they are **not separate published exam domains**.

## How to follow each study day

1. **Learn:** What is it? Why does it exist? Which systems interact with it?
2. **Explain:** Describe the concept in your own words and answer a few questions.
3. **Do:** Complete a guided task, then attempt an independent variation.
4. **Diagnose:** Investigate a broken scenario when safe and applicable.
5. **Prove:** Capture sanitized evidence, check expected vs. actual results, and do exam-style questions.
6. **Record:** Update `PROGRESS.md`; document lessons; review changes before commit/push.

## Phase 0 — Repository and prerequisite foundations

| Day | Focus | Required outcome | Status |
| --- | --- | --- | --- |
| 01 | Personal Git learning repository | Verify directory; initialize Git; create and understand initial docs and `.gitignore`; review, commit, and push | Planned |
| 02 | Linux operations for troubleshooting | Inspect processes, system resources, services and logs; interpret abnormal output | Planned |
| 03 | Docker operations | Inspect images, containers, networking and volumes; troubleshoot a failed container | Planned |
| 04 | Kubernetes architecture and local cluster | Explain control plane and nodes; install kind if appropriate; create **personal** cluster and inspect it | Planned |
| 05 | Kubernetes Pods and deployments | Deploy workload, check status/events/logs, troubleshoot a start failure | Planned |
| 06 | Kubernetes Services and scheduling | Test connectivity and resource scheduling; diagnose an intentionally broken case | Planned |
| 07 | Foundation checkpoint | Independent hands-on task, command interpretation, and cumulative scenario quiz | Planned |

## Phase 1 — Installation and Deployment (31%)

**Target skills:** NVIDIA Base Command Manager (BCM), provisioning and cluster lifecycle, NVIDIA Mission Control, installation/configuration of the relevant cluster software, and validation of deployments.

**Lab approach:** Practice generic provisioning and Kubernetes/Slurm mechanisms locally when possible. Use clearly labeled *simulated* BCM/Mission Control logs and cases when proprietary enterprise infrastructure is unavailable.

**Exit gate:** Diagnose deployment failures from evidence and explain which component or configuration is responsible.

## Phase 2 — Administration (23%)

**Target skills:** Cluster management, Slurm, Kubernetes, NVIDIA Run:ai concepts, GPU allocation/MIG where relevant, administrative operations and access/resource policies.

**Lab approach:** Perform suitable Kubernetes work locally. Use command-output interpretation and *simulated* enterprise GPU/Slurm scenarios when necessary.

**Exit gate:** Explain scheduling and resource decisions, recognize administration failures, and choose the right first diagnostic command.

## Phase 3 — Workload Management (23%)

**Target skills:** Training and inference workload operations, NGC container workflows, resource allocation, scheduling, and practical workload diagnosis.

**Lab approach:** Use small CPU/container workloads for transferable basics. Add GPU labs only after verifying personal hardware, compatible drivers/runtime, and safety of changes.

**Exit gate:** Trace a workload from submission to execution and identify which layer prevents progress.

## Phase 4 — Troubleshooting and Optimization (23%)

**Target skills:** Systematic incident investigation, Docker/cluster faults, NVLink/NVSwitch fabric management, NVIDIA Magnum IO, storage/network/performance symptoms, and optimization evidence.

**Lab approach:** Real local fault injection where safe, plus explicitly *simulated* multi-node and NVIDIA fabric incidents.

**Exit gate:** Apply `Observe → Gather evidence → Isolate layer → Test hypothesis → Fix → Verify` without jumping straight to a guess.

## Phase 5 — Professional-level assessment

- Domain checkpoints: concepts, architectures, command output, failure diagnosis and real/simulated labs.
- Mixed cumulative practice: revisit weak topics from previous phases.
- Timed mock question sets and scenario-based practical drills.
- Record wrong answers and reassess until explanations and execution are consistently strong.

## Daily status rules

Use `Planned`, `In progress`, `Blocked`, or `Completed`. Mark `Completed` only after required evidence and assessment are recorded in `PROGRESS.md`. Add more study days **as the preceding ones are completed** instead of fabricating an entire calendar.
