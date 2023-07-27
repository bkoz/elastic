# elasticsearch-eck-operator-certified

Elastic Cloud on Kubernetes (ECK) is the official operator by Elastic for automating the deployment, provisioning, management, and orchestration of Elasticsearch, Kibana, APM Server, Beats, Enterprise Search, Elastic Agent, Elastic Maps Server, and Logstash on Kubernetes.

Current features:

*  Elasticsearch, Kibana, APM Server, Enterprise Search, Beats, Elastic Agent, Elastic Maps Server, and Logstash deployments
*  TLS Certificates management
*  Safe Elasticsearch cluster configuration and topology changes
*  Persistent volumes usage
*  Custom node configuration and attributes
*  Secure settings keystore updates

Supported versions:

* Kubernetes 1.24-1.27
* OpenShift 4.8-4.12
* Google Kubernetes Engine (GKE), Azure Kubernetes Service (AKS), and Amazon Elastic Kubernetes Service (EKS)
* Elasticsearch, Kibana, APM Server: 7.10+, 8+
* Enterprise Search: 7.10+, 8+
* Beats: 7.10+, 8+
* Elastic Agent: 7.10+, 8+
* Elastic Maps Server: 7.11+, 8+
* Logstash 8.7+

ECK should work with all conformant installers as listed in these [FAQs](https://github.com/cncf/k8s-conformance/blob/master/faq.md#what-is-a-distribution-hosted-platform-and-an-installer). Distributions include source patches and so may not work as-is with ECK.
Alpha, beta, and stable API versions follow the same [conventions used by Kubernetes](https://kubernetes.io/docs/concepts/overview/kubernetes-api/#api-versioning).
See the full [Elastic support matrix](https://www.elastic.co/support/matrix#matrix_kubernetes) for more information.
See the [Quickstart](https://www.elastic.co/guide/en/cloud-on-k8s/2.8/k8s-quickstart.html) to get started with ECK.