# GitHub Action: Run ttyd server

Run ttyd server

```yaml
- uses: zongou/run-ttyd-server@main
  name: Run ttyd server
    with:
        # description: "Credential for basic authentication (format: username:password)", required
      credential: user:${{ inputs.ttyd-credential|| secrets.TTYD_CREDENTIAL }}
      #   # Port for ttyd server, optional, default is 7681
      # port: 7681
      #   # Enable Zmodem support, optional, deafult is true
      # enableZmodem: false
      #   # Enable Trzsz support, optional, default is true
      # enableTrzsz: false
      #   # Enable Sixel support, optional, default is true
      # enableSixel: false

- name: Keep alive
  shell: bash
  run: sleep 6h
```
