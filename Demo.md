# Demo Script

### Pre demo set up
```bash
tanzu apps workload create pre-demo-tjwa -f config/workload.yaml --yes
```

Create a workload

```bash
tanzu apps workload apply tjwa -f config/workload.yaml --tail --yes
```

When it finishes
```bash
tanzu apps workload get tjwa
```

Demo:
 - Create a workload
 - Tail the workload
 - Show TAP GUI:
    - Supply chain of pre-demo-tjwa, show the boxes and the flow
    - Catalog entry -> App live view of pre-demo-tjwa and tjwa
    - APIs page and the docs there
    - Accelerator page and download an accelerator
 - App live reload with IDE Plugin
