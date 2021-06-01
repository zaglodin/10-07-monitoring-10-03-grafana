### Задание 1

![Image of 1st task](/img/1.PNG)

### Задание 2

promql запросы для выдачи этих метрик:
- 100 - (avg by (instance)(irate(node_cpu_seconds_total{mode="idle"}[5m])) * 100)
- avg(node_load1); avg(node_load5); avg(node_load15)
- node_memory_MemFree_bytes
- node_filesystem_avail_bytes

![Image of 2nd task](/img/3.PNG)


### Задание 3

![Image of 2nd task](/img/3.PNG)
![Image of 2nd task](/img/3.1.PNG)

### Задание 4

```
{
    "annotations": {
      "list": [
        {
          "builtIn": 1,
          "datasource": "-- Grafana --",
          "enable": true,
          "hide": true,
          "iconColor": "rgba(0, 211, 255, 1)",
          "name": "Annotations & Alerts",
          "type": "dashboard"
        }
      ]
    },
    "editable": true,
    "gnetId": null,
    "graphTooltip": 0,
    "id": 7,
    "links": [],
    "panels": [
      {
        "alert": {
          "alertRuleTags": {},
          "conditions": [
            {
              "evaluator": {
                "params": [
                  1
                ],
                "type": "gt"

```