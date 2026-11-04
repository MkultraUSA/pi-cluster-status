# pi-cluster-status

The public status page of a self-patching Raspberry Pi k3s cluster.

Rendered and pushed by a Job running inside the cluster (patch-publisher) after every 6-hour CVE scan and after every self-patch action. The cluster scans its own images with trivy, acts on fixable advisories by rebuilding with security fixes and rolling the fleet via ArgoCD — this page shows the verdicts and the timeline.

Machine-readable: `status.json`.
