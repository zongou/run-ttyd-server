# GitHub Action: Run ttyd server

Runs a ttyd server for diagnostics

```yaml
- uses: zongou/run-ttyd-server@0.0.1
  name: Runs a ttyd server for diagnostics
  if: ${{ failure() }}
```
