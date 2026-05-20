# JAX Examples

This directory contains examples for running JAX workloads using Kubeflow Trainer.

## Examples

| Name | Format | Target Hardware | Description |
|------|--------|-----------------|-------------|
| [JAX MNIST CNN](./image-classification/mnist.ipynb) | Notebook | CPU/GPU | Train a convolutional neural network on the MNIST dataset using JAX and Flax. |
| [JAX TPU Smoke Test](./tpu_smoke_test.yaml) | YAML Manifest | TPU (v4, v5e, v6e, v7, v8) | A Kubernetes-native TrainJob manifest that initializes a multi-host distributed JAX cluster on physical Google Cloud TPUs and executes a validation matrix multiplication. |

## Prerequisites

For the YAML example, ensure you have:
1. A Kubernetes cluster with Kubeflow Trainer v2.2+ installed.
2. A Google Cloud GKE TPU node pool (e.g., `ct5p-hightpu-4g` for TPU v5e).
3. The default `clustertrainingruntimes` configured.
