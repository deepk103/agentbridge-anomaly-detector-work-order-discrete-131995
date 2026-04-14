# Architecture Documentation

## Overview
This Reflection implements Anomaly Detector • Work Order (Discrete) for Manufacturing use cases.

## Components
1. **Order Intake**: Collect, validate and normalize downtime events from WMS; attach a runId and timestamp for traceability.
2. **Draft**: Execute draft phase for the Reflection pattern: persist interim state, enforce guardrails, and emit structured JSON results.
3. **Self-Critique**: Execute self-critique phase for the Reflection pattern: persist interim state, enforce guardrails, and emit structured JSON results.
4. **Replenishment**: Replenishment across joined datasets; branch on thresholds using decision gates; write metrics (success/error counts) for observability.
5. **Setup Optimization**: Setup Optimization across joined datasets; branch on thresholds using decision gates; write metrics (success/error counts) for observability.
6. **Defect Detection**: Defect Detection across joined datasets; branch on thresholds using decision gates; write metrics (success/error counts) for observability.
7. **Traceability**: Traceability across joined datasets; branch on thresholds using decision gates; write metrics (success/error counts) for observability.
8. **Maintenance Plan**: Maintenance Plan across joined datasets; branch on thresholds using decision gates; write metrics (success/error counts) for observability.
9. **Quality Summary**: Assemble final payload with status, artifacts, KPIs and audit trail; store to APS; return response JSON for the client.

## Data Flow
- Input: Order Intake
- Processing: 9 sequential steps
- Output: Quality Summary
