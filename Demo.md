# Demo Script

### Pre demo set up
```bash
tanzu apps workload create tanzu-java-web-app -f config/workload.yaml --yes --type web --label app.kubernetes.io/part-of=tanzu-java-web-app --label apps.tanzu.vmware.com/has-tests=true

# tanzu apps workload create node-demo1 --git-repo https://github.com/emosher/node-demo.git --git-branch main --yes
```

### Demo script

Introduce "Joe" for a day in the life

Joe gets the call, deploy that demo app

```
tanzu apps workload create node-demo --git-repo https://github.com/emosher/node-demo.git --git-branch main --type web --yes
```

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

