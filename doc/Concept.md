# Conclusion


| Criteria             | minikube                                                | kind                                            | k3d                              |
| -------------------- | ------------------------------------------------------- | ----------------------------------------------- | -------------------------------- |
| Case of use          | localhost development                                   | optimized for CI pipelines                      | used mainly IoT and Edge devices |
| Cluster Type         | Single-node                                             | Single-node, multi-node                         | Single-node, multi-node          |
| Resource Consumption | Higher                                                  | Lower                                           | Lowest                           |
| Podman Support       | Community workarounds                                   | Yes                                             | Limited community exploration    |
| Container Runtime    | Docker ( default ) configurable for containerd or CRI-O | Docker ( default ), configurable for containerd | Docker (only)                    |

![Image](../.data/kind.gif)
Based on the comparison table, Kind seems like the best choice for a local Kubernetes cluster tool for usage on localhost. It has lower resource requirements, making it more efficient, and offers easier integration with CI/CD pipelines. Additionally, Kind supports creating multi-node clusters, which provides more flexibility for testing purposes.