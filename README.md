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

### Current / expected volume (Builder counters)
- Bot 5m: **DAY $12,646.05 | WEEK $21,102.24**
- Bot 15m: **DAY $33,836.37 | WEEK $73,547.20**
- Bot 1h: **DAY $23,374.50 | WEEK $67,591.11**
- TOTAL (sum): **DAY $69,856.92 | WEEK $162,240.55**

### Security & operations (high level)
- Non-custodial signing (EIP-712); secrets are never committed
- Sanitized logs; no infrastructure identifiers published
- Happy to share additional logs/metrics privately upon request

### Contact
- Maintainer: JorgeCIC
- Email: *(Provided privately in the official Polymarket Builder application / email thread)*
- Telegram: *(Provided privately via email thread)*

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

### Volumen actual / esperado (contadores Builder)
- Bot 5m: **DAY $12,646.05 | WEEK $21,102.24**
- Bot 15m: **DAY $33,836.37 | WEEK $73,547.20**
- Bot 1h: **DAY $23,374.50 | WEEK $67,591.11**
- TOTAL (suma): **DAY $69,856.92 | WEEK $162,240.55**

### Contacto
- Responsable: JorgeCIC
- Email: Email: (Proporcionado por vía privada en la solicitud oficial / hilo de email)
- Telegram: (Proporcionado por vía privada en el hilo de email)
  
