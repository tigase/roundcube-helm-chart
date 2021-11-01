# Roundcube Helm Chart

This Helm chart allows for an easy install of [Roundcube webmail client](https://roundcube.net/) to your Kubernetes cluster.

## Installation

### Add Helm Repository

```
helm repo add mlohr https://helm-charts.mlohr.com/
helm repo update
```

### Create Minimal Configuration

In order to get Roundcube running, you need to provide the following minimal configuration.
For a full documentation of all possible configuration options, check the [values.yaml file](https://gitlab.com/MatthiasLohr/roundcube-helm-chart/-/blob/main/values.yaml).

Your `values.yaml`:
```yaml
ingress:
  host: roundcube.your.domain

imap:
  host: imap.your.domain

smtp:
  host: smtp.your.domain

externalDatabase:
  type: pgsql
  host: db.your.domain
  name: roundcube
  user: roundcube
  password: S3cret!
```


### Install to Kubernetes

```bash
helm install roundcube mlohr/roundcube -f values.yaml
```


## Links
  * https://roundcube.net/
  * https://github.com/roundcube/roundcubemail
  * https://github.com/roundcube/roundcubemail-docker
