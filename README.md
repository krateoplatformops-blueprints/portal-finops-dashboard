# FinOps Dashboard
This is the composable FinOps dashboard.

## Requirements
- Krateo >= 2.5.1

## How to install

```sh
helm install <name> portal-finops-dashboard \
  --repo https://marketplace.krateo.io \
  --namespace <krateo-namespace> \
  --version 1.0.0 \
  --wait
```

# Resource Tree
[NavMenuItem nav-menu-item-dashboard-finops](chart/templates/navmenuitem.nav-menu-item-finops-dashboard.yaml)
- [Page finops-dashboard-page](chart/templates/pages.finops-dashboard-page.yaml)

[Page finops-dashboard-page](chart/templates/pages.finops-dashboard-page.yaml)
- [Panel finops-dashboard-summary-panel](chart/templates/panel.finops-dashboard-summary-panel.yaml)
- [Panel finops-dashboard-compositions-panel](chart/templates/panel.finops-dashboard-compositions-panel.yaml)

[Panel finops-dashboard-summary-panel](chart/templates/panel.finops-dashboard-summary-panel.yaml)
- [Row finops-dashboard-summary-panel-row-1](chart/templates/row.finops-dashboard-summary-panel-row-1.yaml)
- [Paragraph finops-dashboard-summary-panel-row-2-paragraph](chart/templates/paragraph.finops-dashboard-summary-panel-row-2-paragraph.yaml)

[Panel finops-dashboard-compositions-panel](chart/templates/panel.finops-dashboard-compositions-panel.yaml)
- [Table finops-dashboard-compositions-panel-table](chart/templates/table.finops-dashboard-compositions-panel-table.yaml)
  - [RestAction finops-dashboard-compositions-panel-table](chart/templates/restaction.finops-dashboard-compositions-panel-table.yaml)

[Row finops-dashboard-summary-panel-row-1](chart/templates/row.finops-dashboard-summary-panel-row-1.yaml)
- [PieChart finops-dashboard-summary-panel-row-1-piechart](chart/templates/widget.finops-dashboard-summary-panel-row-1-widgets.yaml)
  - [RestAction finops-dashboard-summary-panel-row-1-piechart](chart/templates/restaction.finops-dashboard-summary-panel-row-1-widgets.yaml)
- [LineChart finops-dashboard-summary-panel-row-1-piechart](chart/templates/widget.finops-dashboard-summary-panel-row-1-widgets.yaml)
  - [RestAction finops-dashboard-summary-panel-row-1-linechart](chart/templates/restaction.finops-dashboard-summary-panel-row-1-widgets.yaml)