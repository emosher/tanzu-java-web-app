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

```bash
tanzu apps workload apply tjwa -f config/workload.yaml --tail --yes
```

When it finishes
```bash
tanzu apps workload get tjwa
```




Demo:
 - Create workload before demo
 - Create a workload
 - Tail the workload
 - Show TAP GUI:
    - Accelerator page and download an accelerator
    - Supply chain of pre-demo-tjwa, show the boxes and the flow
    - Catalog entry -> App live view of pre-demo-tjwa and tjwa
    - APIs page and the docs there 
 - App live reload with IDE Plugin
