# Sample ElasticSearch Client

Login to the Openshift cluster to obtain the authentication credentials and 
routing information needed to connect to ElasticSearch.

Example `bash` commands to be run with `cluster-admin` privledges.

```
oc get routes elastic -o=jsonpath='{.spec.HOST}'
oc get secrets elasticsearch-sample-es-elastic-user -o=jsonpath='{.data.elastic}' | base64 --decode
```

### Python snippets.

```
import subprocess

COMMAND = "oc whoami --show-context"
logging.info("Openshift context: %s", subprocess.check_output(COMMAND, shell=True).decode())

COMMAND = "oc get routes elastic -o=jsonpath='{.spec.ELASTIC_HOST}'"
ELASTIC_HOST = subprocess.check_output(COMMAND, shell=True).decode()

COMMAND = "oc get secrets elasticsearch-sample-es-elastic-user \
    -o=jsonpath='{.data.elastic}' | base64 --decode"
ELASTIC_PASSWORD = subprocess.check_output(COMMAND, shell=True).decode()
```
