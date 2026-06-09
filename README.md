# Payroll Command Center

A localized, local-first web utility engineered for tracking timecard matrices, forecasting biweekly payroll distributions, and monitoring multi-tier pre-tax and post-tax accounting workflows directly from the browser. Fully optimized for 6.1" dynamic viewports (`iPhone 14 Pro`).

## Architectural Parameters

- **Base Rate Verification:** Default structural baseline set to `$41.64/hr`.
- **Shift Matrix Execution:** 12-hour shifts mapped to regular time (`Reg`), Overtime (`OT`), and double-time (`DT`) Sunday system parameters.
- **Pay Period Sequencing:** Structured drop-downs configured exclusively for biweekly pay periods initializing on **Mondays**.
- **Data Privacy Frame:** Local-first engineering pattern. System telemetry and timecard state are persistently written directly to client-side `localStorage`. Zero third-party cloud synchronizations or analytics vectors.

## Core Features
- **Timecard Module:** Individual toggle switches for Emergency PTO (`EPTO`) allocations that cleanly drop core shifts to baseline parameters.
- **Calendar Matrix Module:** Tracks planned month-level leave metrics alongside premium system-coverage parameters (1.5x premium indexing logic).
- **Tax Verification Engine:** Integrated state withholding baselines calculated on the Georgia tax schedule framework (`4.99%`) along with standard simple FICA allocations (`6.2%` SS, `1.45%` Medicare) and an optional toggled Federal baseline (`8.2%`).

## Initialization & Use
Simply serve `index.html` locally using any standard localized daemon or static launcher:

```bash
# Example via Python static daemon
python3 -m http.server 8080
