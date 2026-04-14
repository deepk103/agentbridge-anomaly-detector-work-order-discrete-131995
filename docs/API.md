# API Documentation

## Endpoints
### Order Intake
- **Description**: Collect, validate and normalize downtime events from WMS; attach a runId and timestamp for traceability.
- **Type**: Processing

### Draft
- **Description**: Execute draft phase for the Reflection pattern: persist interim state, enforce guardrails, and emit structured JSON results.
- **Type**: Processing

### Self-Critique
- **Description**: Execute self-critique phase for the Reflection pattern: persist interim state, enforce guardrails, and emit structured JSON results.
- **Type**: Processing

### Replenishment
- **Description**: Replenishment across joined datasets; branch on thresholds using decision gates; write metrics (success/error counts) for observability.
- **Type**: Processing

### Setup Optimization
- **Description**: Setup Optimization across joined datasets; branch on thresholds using decision gates; write metrics (success/error counts) for observability.
- **Type**: Processing

### Defect Detection
- **Description**: Defect Detection across joined datasets; branch on thresholds using decision gates; write metrics (success/error counts) for observability.
- **Type**: Processing

### Traceability
- **Description**: Traceability across joined datasets; branch on thresholds using decision gates; write metrics (success/error counts) for observability.
- **Type**: Processing

### Maintenance Plan
- **Description**: Maintenance Plan across joined datasets; branch on thresholds using decision gates; write metrics (success/error counts) for observability.
- **Type**: Processing

### Quality Summary
- **Description**: Assemble final payload with status, artifacts, KPIs and audit trail; store to APS; return response JSON for the client.
- **Type**: Processing
