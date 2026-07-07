## ArgoCD Applications per EKS Cluster

```
│
├── HelmCharts             # All Helm Charts
│   ├── ChartTest1
│   │   ├── Chart.yaml
│   │   ├── templates
│   │   ├── values_dev.yaml    # DEV Values
│   │   ├── values_prod.yaml   # PROD Values
│   │   └── values.yaml        # Default Values
│   └── ChartTest2
│       ├── Chart.yaml
│       ├── templates
│       ├── values_dev.yaml    # DEV Values
│       ├── values_prod.yaml   # PROD Values
│       └── values.yaml        # Default Values
│   
└── my-cluster               # EKS Cluster name
    ├── dev
    │    ├── applications
    │    │   ├── app1.yaml
    │    │   └── app2.yaml
    │    └── root.yaml              # Root ArgoCD Application
    └── prod
        ├── applications
        │   ├── app1.yaml
        │   └── app2.yaml
        └── root.yaml              # Root ArgoCD Application    
```