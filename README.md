# README: Dynatrace Deployment

This document provides a step-by-step guide for deploying Dynatrace on Kubernetes and managing deployment statuses, including the installation of ActiveGates.

---

## Overview

### Purpose:
- Guide for setting up Dynatrace ActiveGates and deploying Dynatrace on Kubernetes.

### Prerequisites:
1. Access to your Kubernetes cluster.
2. Dynatrace account credentials.
3. API and PaaS tokens.

---

## Section 1: Manage Deployment Status - Install ActiveGates

### Instructions:
1. Follow the steps outlined for installing ActiveGates on your instance.

---

## Section 2: Deploy Dynatrace on Kubernetes

### Instructions:
1. Navigate to the Dynatrace interface and click on **"Start Installation"**.
2. Select **Kubernetes** as the deployment type.

#### Configuration:
1. **Token Setup:**
   - Either create a new token or use an existing one. API and PaaS tokens will be the same.
2. **Cluster Setup:**
   - Provide a unique **Cluster Name**.
   - Specify a **Group Name**.
   - Enable **SSL Check**.
3. Download the `dynakube.yaml` configuration file.

#### Deployment Commands:
1. Create the namespace for Dynatrace:
   ```bash
   kubectl create namespace dynatrace
   ```
2. Label the namespace for Dynatrace injection:
   ```bash
   kubectl label namespace docs-kube-prod dynatrace.com/inject=true
   ```
3. Apply the Dynatrace operator:
   ```bash
   kubectl apply -f https://github.com/Dynatrace/dynatrace-operator/releases/download/v1.4.0/kubernetes.yaml
   ```
4. Wait for the operator webhook to be ready:
   ```bash
   kubectl -n dynatrace wait pod --for=condition=ready --selector=app.kubernetes.io/name=dynatrace-operator,app.kubernetes.io/component=webhook --timeout=300s
   ```
5. Apply the Dynakube configuration file:
   ```bash
   kubectl apply -f dynakube_application.yaml
   ```
6. Create a Kubernetes secret for the API token:
   ```bash
   kubectl -n dynatrace create secret generic dynakube --from-literal="apiToken=YOUR_API_TOKEN"
   ```

#### Final Steps:
1. Go to the **Kubernetes** section in Dynatrace by searching for "Kubernetes" in the search bar.
2. Wait for the cluster to appear in the Dynatrace interface.

---

## Notes
- Ensure SSL checks are enabled for secure communication.
- Use the provided commands as-is or customize them based on your infrastructure setup.

For further assistance, refer to the official Dynatrace documentation.

