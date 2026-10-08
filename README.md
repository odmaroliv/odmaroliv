## Odmar Olivares

CTO of a cross-border logistics operation between San Diego, Tijuana and
Los Cabos. I build the systems that move freight across the border:
warehouse software, fleet tracking, vehicle video, and the security around
them.

### Now: [OpenMDVR](https://github.com/openmdvr/openmdvr)

A self-hosted fleet video and GPS platform, open source under Apache-2.0.
I designed and built it end to end.

It started with a gap I hit running our own GPS platform: open-source
tracking servers did not support dashcams, so fleet video meant a closed
third-party service. If you self-host everything, that was a dead end.
OpenMDVR is the answer.

- Device servers in Go for JT/T 808, JT/T 1078 and the GT06 family.
- Live dashcam video in the browser over WebRTC with audio, authorized
  with one-time tickets.
- Tenant isolation enforced inside PostgreSQL with Row Level Security,
  hardened through adversarial security reviews.
- Load tested at 50,000 simulated trackers on a 2 vCPU server, with every
  position stored. Along the way I found and fixed a PostgreSQL commit
  bottleneck that capped ingestion at about 550 positions per second.

### Other work

- **WMSARN.** Warehouse management for binational 3PL distribution:
  receiving, inventory, putaway and RFID. FastAPI and PostgreSQL, in
  production since 2024, built with the team I lead.
- **Tracknel.** Our GPS fleet tracking platform, re-architected on Traccar
  and TimescaleDB. It cut operating cost by more than 80% with no loss of
  coverage, and it is where OpenMDVR began.
- **C-TPAT certification.** Led the company's certification with U.S.
  Customs and Border Protection, from security policy to physical audits.

### What I work with

Go, Python (FastAPI), C# / ASP.NET, PostgreSQL and TimescaleDB, Docker,
React and TypeScript, Flutter and Dart. Binary device protocols, real-time
video (WebRTC, RTMP), multi-tenant security.

### Links

[odmardaniel.com](https://odmardaniel.com/) ·
[LinkedIn](https://www.linkedin.com/in/odmarolivares/)
