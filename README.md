# Test Helm Repository

This is a test Helm repository with multiple charts designed to test Helm v4 breaking changes.

## Charts Included

1. **nginx-test** (v1.0.0) - Valid chart
2. **redis-test** (v1.0.0) - Valid chart
3. **broken-chart** (v1.0.0) - Invalid/corrupted chart for testing error handling

## Usage

Add this repository to your Helm:
```bash
helm repo add test-repo https://raw.githubusercontent.com/CJkrishnan/TestRepo/main/
helm repo update
```

## Purpose

This repository is specifically designed to test:
- Helm v4 behavior with `helm repo update` when charts have issues
- CD/RO EC-Helm plugin error handling
- Repository update failures and partial successes