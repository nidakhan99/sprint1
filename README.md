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
   - Enable **SSL Check**.(optinal)
3. Download the `dynakube.yaml` configuration file.

#### Deployment Commands:
1. Use Helm to install the Dynatrace operator:
   ```bash
   helm install dynatrace-operator oci://public.ecr.aws/dynatrace/dynatrace-operator \
       --create-namespace \
       --namespace dynatrace \
       --atomic
   ```
2. Apply the downloaded configuration file:
   ```bash
   kubectl apply -f dynakube.yaml
   ```
3. Create a Kubernetes secret for the API token:
   ```bash
   kubectl -n dynatrace create secret generic dynakube --from-literal="apiToken=hhwdude"
   ```

#### Final Steps:
1. Go to the **Kubernetes** section in Dynatrace by searching for "Kubernetes" in the search bar.
2. Wait for the cluster to appear in the Dynatrace interface.

---

## Notes
- Ensure SSL checks are enabled for secure communication.
- Use the provided commands as-is or customize them based on your infrastructure setup.

For further assistance, refer to the official Dynatrace documentation.

