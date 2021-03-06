## Why

Given that application configurations for Kubernetes software can be specified in various forms:

- plain YAML configurations
- Helm charts
- ytt templates
- jsonnet templates
- etc.

and found in various locations:

- Git repository
- Archive over HTTP
- Helm repository
- etc.

and written/provided by:

- in-house development teams
- vendors offering COTS products

as a Kubernetes user I would like to customize, install, and update such software in a _consistent_ and _manageable_ manner.

kapp-controller provides a Kubernetes native way, via App CRD, to specify how to fetch, configure and deploy software to the cluster.

Another motivation for kapp-controller was to make a small and single purpose system (as opposed to a general CD system); hence, it's lightweight, easy-to-understand and easy-to-debug. It builds on small composable tools to achieve its goal and therefore is easy to think about.

Finally, for the fans of GitOps, kapp-controller turns [kapp](https://get-kapp.io) into your continuous cluster reconciler.

Next: [Install](install.md)
