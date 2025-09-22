# _FinOps Dashboard_ Blueprint
The FinOps Dashboard Blueprint provides a ready-to-use page to monitor Krateo's resources and their costs, with warnings related to underutilized resources. This Blueprint includes a Helm chart to help you bootstrap your own Krateo Composable Portal and Krateo Composable FinOps experience.

## What It Does
This blueprint deploys a new menu option that offers a FinOps dashboard, allowing you to quickly visualize all your costs and the specifics costs of your compositions. The dashboard includes:
- Costs summary by category;
- Costs timeline;
- List of compositions with the their respective utilization, cost and underutilization warning.

## Install the Helm Chart

Install the Blueprint:

```sh
helm install <name> portal-finops-dashboard \
  --repo https://marketplace.krateo.io \
  --namespace <krateo-namespace> \
  --version 1.0.0 \
  --wait
```

The FinOps Dashboard **must** be installed in the Krateo Namespace. If you install using Helm, then you must set `.Values.global.krateoNamespace` to the Krateo namespace.