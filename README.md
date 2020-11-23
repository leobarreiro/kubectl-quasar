# Kubectl Quasar [![Kubernetes](https://img.shields.io/badge/kubernetes-openidconnect-orange)](https://kubernetes.io/docs/reference/access-authn-authz/authentication/#openid-connect-tokens) [![Kubectl](https://img.shields.io/badge/kubectl-plugins-green)](https://kubernetes.io/docs/reference/kubectl/) [![Python 3](https://img.shields.io/badge/python-3-9cf)](https://www.python.org/) 

**kubectl-quasar** is a set of tools to use with kubectl. Writen in _python3_, **kubectl-quasar** runs as a plugin into kubectl, adding to him some functionalities:

- quasar login - allows perform a simple login against any openid oath2 authorization server (like keycloak, for example).

```
$ kubectl quasar login -u my-user -p my-password
```

- quasar config - configures a new credential (or edit an existing) into kubectl, based on openidconnect protocol. 

```
$ kubectl quasar config
```