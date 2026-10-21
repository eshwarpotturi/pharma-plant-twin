# Tablet Plant Twin

**▶ Live demo: https://eshwarpotturi.github.io/pharma-plant-twin/**

A 3D digital twin of an oral solid dose (tablet) plant, with an AI agent that finds a delayed batch, traces the cause, fixes what it is allowed to, and asks a person before anything costly.

Proof of concept for Straive's Innovation Team, adapted from the [transformer plant twin](https://github.com/eshwarpotturi/transformer-plant-twin). **All data is synthetic.** Figures are typical industry values, not any client's.

## Guided demo

Click **▶ Play demo**. Six steps, one line each, written to be read aloud:

1. A tablet plant with 25 batches in flight
2. Midnight · a 4-day backlog at Tablet press 2
3. …because Coating pan 1 is running slow
4. The agent sends the spare pump itself, then asks to fit it *(approval 1)*
5. It won't skip a QC release test, so it asks for an extra lab shift *(approval 2)*
6. Two weeks later · what the agent saved

## The plant

Warehouse and dispensing → granulation (Grade C) → fluid-bed drying → tablet presses → film coating → QC release lab → packaging and dispatch, plus utilities, maintenance, microbiology lab and planning office. Click any building or machine for what it does, its capacity and what it is working on now.

## Agent rules

- **Does it alone, then reports:** supplier follow-ups, re-ordering queues, moving spare parts, booking internal resources.
- **Asks a person first:** taking equipment offline, overtime above ₹2 L, purchases above ₹50 L, anything sent to a customer or regulator.
- **Never allowed:** skipping or shortening a QC test, releasing a batch without QA sign-off, shipping a batch that failed a test.
