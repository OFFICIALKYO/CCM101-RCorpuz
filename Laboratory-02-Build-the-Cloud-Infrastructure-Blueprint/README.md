# Laboratory 02 - Build the Cloud Infrastructure Blueprint

## Mission Overview
Assessed a Linux server running in KillerCoda as part of a simulated cloud migration planning phase, documenting its compute, storage, networking, and OS resources, and comparing equivalent services across AWS, Azure, and GCP.

## Objectives
- Explain the major components of cloud infrastructure
- Investigate hardware and software resources in a Linux environment
- Differentiate compute, storage, networking, and identity resources
- Create professional technical documentation using Markdown
- Continue building a structured GitHub Cloud Computing Portfolio

## Cloud Infrastructure Components
| Component | Linux Evidence |
|---|---|
| Compute | `nproc`, `lscpu`, `free -h` |
| Storage | `df -h`, `lsblk` |
| Networking | `ip addr`, `hostname -I` |
| Operating System | `/etc/os-release`, `uname -r` |

See [cloud-components.md](cloud-components.md) and [infrastructure-report.md](infrastructure-report.md).

## Tools Used
- KillerCoda Playground
- Git and GitHub
- Markdown
- Draw.io / Excalidraw (diagram)

## Linux Commands Executed
```bash
cat /etc/os-release
uname -r
hostname
hostname -I
lscpu
nproc
free -h
df -h
df -hT
lsblk
ip addr show
```

## Skills Learned
- Inspecting system resources using Linux commands
- Mapping Linux resources to cloud infrastructure concepts
- Comparing AWS, Azure, and GCP services
- Writing structured technical documentation in Markdown
- Committing work to GitHub per checkpoint

## Challenges Encountered
(Write your real challenges here, e.g. Git push authentication, finding the right commands, diagram export.)

## Deliverables
- [infrastructure-report.md](infrastructure-report.md)
- [cloud-components.md](cloud-components.md)
- [cloud-provider-comparison.md](cloud-provider-comparison.md)
- [reflection.md](reflection.md)
- `screenshots/`
