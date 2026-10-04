# kubernetes-production-patterns

> Hardened Kubernetes manifests using Kustomize, pod security standards, Horizontal Pod Autoscaling (HPA), and multi-environment overlays.

> [!NOTE]
> This repository is a production reference implementation. Manifests demonstrate cloud-native best practices and are not automatically deployed to a live cluster in this portfolio repository.

## Highlights
- **Pod Security Standards**: Non-root UID, read-only root filesystems, dropped Linux capabilities.
- **Zero-Downtime Updates**: `RollingUpdate` with `maxSurge: 1` and `maxUnavailable: 0`.
- **Autoscaling**: HorizontalPodAutoscaler targeting 70% CPU threshold.
- **Kustomize Overlays**: Environment customization between `base` and `overlays/production`.

## Author
**Manish Lalotra**  
Full Stack Developer & DevOps Engineer  
*Full Stack Developer | DevOps Engineer | Cloud & Infrastructure Engineer*

## License
MIT License. See [LICENSE](LICENSE) for details.
