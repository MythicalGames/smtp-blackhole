# SMTP Blackhole Container

This container is useful for testing OpenUnison without an email server available for notifications.

# Running

Assuming Kubernetes with the namespace `blackhole`:

```
$ kubectl create deployment blackhole --image=tremolosecurity/smtp-blackhole -n blackhole
$ kubectl expose deployment/blackhole --type=ClusterIP --port 1025 --target-port=1025 -n blackhole
```

