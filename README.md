# Rubin — Public One-Pager (Verification)

Rubin is a Node.js system for automated execution and order management on Polymarket’s CLOB, built with conservative operational controls and isolated production nodes.

---

## English

### What Rubin does (today)
- **Production today (FAK):** automated execution using **FAK (Fill-or-Kill)** orders
- Defined **execution cadence** and order management; **no resting orders**
- **Three independent nodes:** 1h, 15m, 5m
- Each node is isolated with its own **wallet/account**, **Builder Profile/ID**, and **Builder API key**

### Roadmap (GTC/GTD quoting — not live yet)
- Deploy resting limit-order quoting on eligible markets under the **Liquidity Rewards** program
- **Target** consistent two-sided depth near the midpoint, within per-market max-spread and min-size parameters
- Practical goal: tighten spreads and improve execution quality with conservative risk controls
- Note: eligibility and parameters are market-specific and defined by Polymarket

### Why we’re requesting Verified tier
- Current tier: **Unverified (100 relayer tx/day)**
- The **5m node** needs **~288+ relayer tx/day** for basic order management / execution cadence
- At 100 tx/day we hit relayer rate-limits, degrading normal operation

### Current / expected volume (for attribution)
- Bot 5m: **DAY $12,399.75 | WEEK $19,858.50**
- Bot 15m: **DAY $32,785.67 | WEEK $69,268.25**
- Bot 1h: **DAY $24,394.74 | WEEK $64,796.80**
- TOTAL: **DAY $69,580.16 | WEEK $153,923.55**

### Builder profiles (public placeholders)
- **[WALLET_1] — [BUILDER_ADDRESS_1] — [BUILDER_KEY_1]**
- **[WALLET_2] — [BUILDER_ADDRESS_2] — [BUILDER_KEY_2]**
- **[WALLET_3] — [BUILDER_ADDRESS_3] — [BUILDER_KEY_3]**

### Security & operations (high level)
- Non-custodial signing (EIP-712); secrets are never committed
- Sanitized logs; no infrastructure identifiers published
- Happy to share additional logs/metrics privately upon request

### Contact
- Maintainer: **[MI ALIAS]**
- Email: **[EMAIL]**
- Telegram: **[TELEGRAM]**

---

## Español

### Qué hace Rubin (hoy)
- **Producción (FAK):** ejecución automatizada con órdenes **FAK (Fill-or-Kill)**
- Cadencia de ejecución y gestión de órdenes; **sin órdenes resting**
- **Tres nodos independientes:** 1h, 15m, 5m
- Cada nodo aislado con su **wallet/cuenta**, **Builder Profile/ID** y **Builder API key**

### Roadmap (quoting GTC/GTD — aún no está en producción)
- Desplegar quoting con órdenes limit resting en mercados elegibles del programa **Liquidity Rewards**
- **Apuntar** a profundidad bid/ask cerca del midpoint, respetando max-spread y min-size por mercado
- Objetivo práctico: reducir spreads y mejorar la calidad de ejecución con controles de riesgo conservadores
- Nota: la elegibilidad y parámetros son por mercado y los define Polymarket

### Motivo del upgrade
- Tier actual: **Unverified (100 relayer tx/day)**
- El nodo **5m** requiere **~288+ relayer tx/day** para rutinas básicas
- Con 100 tx/day aparecen rate-limits y se degrada la operativa

### Contacto
- Responsable: **[MI ALIAS]** — **[EMAIL]** — **[TELEGRAM]**

> Nota: este README es intencionalmente de alto nivel (sin código, sin detalles operativos sensibles, sin secretos).
