# Demo Script

### Pre demo set up
```bash
tanzu apps workload create pre-demo-tjwa -f config/workload.yaml --yes
```

Start the `Tiltfile`

### Commands used in demo

Create a workload

```bash
tanzu apps workload apply tjwa -f config/workload.yaml --tail --yes
```

When it finishes
```bash
tanzu apps workload get tjwa
```

Strings used, for easy copy/paste
```
"Greetings from Spring Boot and Tanzu!!!"
"This is a test!"
"Hey, I hope this works!!"
```

Demo:
 - Create a workload and tail it
 - Show TAP GUI:
    1. Supply chain of pre-demo-tjwa, show the boxes and the flow of a completed supply chain
    1. Catalog entry of tjwa
    2. App live view of pre-demo-tjwa and tjwa
    3. APIs page and the docs there
    4. Accelerator page and download an accelerator
 - IDE Plugin and app iteration
