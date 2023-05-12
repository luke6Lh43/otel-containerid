# otel-containerid

This is a simple solution that creates ConfigMap with OTEL_SERVICE_NAME to corresponding container ID mapping.

To verify how it works, please wait a while (CronJob runs every 5 minutes) and execute command:

```
kubectl describe configmap servicename-to-containerid-mapping-configmap -n mynamespace
```
