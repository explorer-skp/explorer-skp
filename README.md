# Soumyakanta Panda

I build **storage, query, and consensus systems from scratch — and I measure
them honestly.** The interesting part is never the demo; it's the tail latency
and the test that can actually fail.

What pulls me is the engineering backbone of finance: low-latency C++ trading
infrastructure and quantitative systems - which is why these projects keep
landing on order books, tick data, and microsecond tails.

CSE @ IIT Patna ('27) · Quant Dev Intern @ 26Miles Capital
→ **[portfolio &amp; benchmarks](https://explorer-skp.github.io)**

### Selected work

- **[raft-rsm](https://github.com/explorer-skp/raft-rsm)** — C++20 Raft from
  scratch (no consensus / RPC / lock-free libraries) carrying a KV store and a
  price-time-priority order-book matcher behind one interface. Commit 199µs p99,
  69K writes/s, 277ms p50 failover; verified by seeded chaos, a linearizability
  checker, and safety invariants that each ship a must-flag self-test. *(shipped)*
- **Vectorized columnar query engine** — typed column batches through portable
  SIMD operators (Google Highway), validated **byte-for-byte against DuckDB** by
  a self-validated differential oracle (17-entry mutation catalog). As-of joins,
  time windows, Gorilla compression; one source → NEON + AVX-512.
  [[details](https://explorer-skp.github.io)] *(building)*
- **Deduplicating snapshot engine** — content-addressed Merkle-DAG snapshots; a
  Mac client and a Linux server dedupe the same bytes to one physical copy and
  agree on the same root across ISAs. [[details](https://explorer-skp.github.io)]
  *(in design)*

### How I work

- **Checkers that can fail.** A checker that cannot fail proves nothing — each is
  fed a deliberately broken system and must flag it.
- **Tails, not averages.** p50 / p99 / p99.9 with coordinated-omission
  correction whenever latency is measured under load.
- **Reproducible.** One command regenerates the data; plots regenerate from saved
  JSON; host and seed recorded so any result replays.

### Elsewhere

2× ICPC Asia Regionalist (All India Rank 18) · Meta Hacker Cup 2025 · JPMC Code
for Good 2025 Finalist · Codeforces Expert (max 1811) ·
[codeforces](https://codeforces.com/profile/explorer_skp) ·
[codechef](https://www.codechef.com/users/explorer_skp) ·
[linkedin](https://www.linkedin.com/in/soumyakanta-panda-1823a3288/)

> *if not now, when*
