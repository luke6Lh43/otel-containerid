# otel-containerid

This is a simple solution that creates ConfigMap with OTEL_SERVICE_NAME to corresponding container ID mapping. It's currently hardcoded for containerd, so it won't work on other container runtimes.

To verify how it works, please deploy all manifests from infra directory, wait a while (CronJob runs every 5 minutes) and execute command:

```
kubectl describe configmap servicename-to-containerid-mapping-configmap -n mynamespace
```
