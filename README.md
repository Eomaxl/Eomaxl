# Sourav Snigdha Mansingh

**Staff Software Engineer — payments, fraud and risk systems**
Go · Java · Python · Kafka · Distributed systems · Applied ML

---

## What I work on

I build the systems that move money — and lately, the ML that
decides whether the money should move at all.

Eleven years across the length of a bank: KYC and customer
onboarding, real-time payment initiation and settlement, ACH and
card scheme processing, credit risk and loan origination. Currently
at Q2, building AI-driven fraud and anomaly detection across ACH
payment, batch and collection flows — catching suspicious activity
before settlement, not in next-day reconciliation.

Before that: Confluent (led a real-time intelligence platform from
zero to MVP in five months), Cisco, DBS Bank, American Express
transaction processing, and a Swiss retail bank.

Open to Staff / Senior Backend roles. Currently exploring
opportunities in the UK.

📩 sourav.mansingh5@gmail.com
🔗 [LinkedIn](https://www.linkedin.com/in/sourav-snigdha-mansingh/)
🌐 [souravmansingh.com](https://www.souravmansingh.com/)
✍️ [Medium](https://souravsnigdha.medium.com/)

---

## Selected work

### [PaymentServiceProvider](https://github.com/Eomaxl/PaymentServiceProvider)
**The full transaction lifecycle — initiation, authorisation, capture, refund**

A distributed payment platform built the way a real one has to be:
idempotency keys so a retried request never double-charges, saga
orchestration so a half-completed payment can always be unwound,
and Kafka for the async legs that must not block the customer.

The hard part isn't throughput — it's being wrong safely.

`Java` · `Spring Boot` · `Kafka` · `PostgreSQL`

---

### [RiskPulse](https://github.com/Eomaxl/RiskPulse)
**Scoring a transaction's risk while it's still in flight**

Tiered fraud scoring over a streaming transaction feed — a fast
gradient-boosted model for the common case, escalating to sequence
and graph models where the signal warrants it. Adverse-media
sentiment from SentimentPulse feeds in as an optional feature.

`Python` · `Kafka` · `XGBoost` · `FastAPI`

---

### [SentimentPulse](https://github.com/Eomaxl/SentimentPulse)
**Real-time financial news sentiment, end to end**

Ingestion through to a live dashboard: Kafka pipeline, a FinBERT
model fine-tuned on financial text (0.92 F1, published on
[Hugging Face](https://huggingface.co/EomaxlSam/finbert-finetuned-sentimentpulse)),
TimescaleDB for the time series, FastAPI and React on top.

Built during a deliberate break from full-time work, to learn what
it actually takes to put a model in a pipeline rather than a
notebook.

`Python` · `Kafka` · `FinBERT` · `TimescaleDB` · `React`

---

### [Real-Time-Chat-Platform](https://github.com/Eomaxl/Real-Time-Chat-Platform)
**Messaging, presence and WebRTC signalling**

Goroutine-per-connection, Redis pub/sub for cross-node fanout,
Postgres for durable history. Written to get properly fluent in
Go's concurrency model.

`Go` · `WebSocket` · `Redis` · `PostgreSQL`

---

## Stack

| | |
|---|---|
| **Languages** | Go, Java, Python |
| **Messaging** | Kafka, Flink, Temporal |
| **Data** | PostgreSQL, Cassandra, Redis, TimescaleDB, pgvector |
| **Infra** | Kubernetes, Docker, AWS, gRPC, Envoy |
| **ML** | PyTorch, HuggingFace, XGBoost, RAG, LangChain |

---

## Writing

I write about distributed systems, payments architecture and
applied ML on [Medium](https://souravsnigdha.medium.com/).
