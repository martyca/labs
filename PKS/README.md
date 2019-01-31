# PKS labs

PKS is a product that offers consumers a container runtime (Kubernetes), focussed on operational effiency by leveraging BOSH, and security by leveraging VMware NSX-T.

## Deployment

In principle the PKS installation is pretty straightforward, given you have a vSphere and NSX-T setup, you can follow the [PKS installation docs](https://docs.pivotal.io/runtimes/pks/1-3/index.html).

However, if you run into issues during installation, you may quickly find the OpsManager GUI is not sufficient, and you'll have to resort to CLI and BOSH.

Below you find the steps you want to ideally take to understand the entire stack. Depending on your previous expertise and environment, you can skip certain steps, although it's highly recommended to go through the whole exercise once.
- [Deploy vSphere](../vSphere/)
- [Deploy NSX-T](../NSX-T/)
- [Understand BOSH](../BOSH/)
- Deploy PKS

After deployment, you will want to prove it works by deploying some workloads.

## Consuming PKS (deploying workloads)

PKS to the consumer is vanilla Kubernetes, to find our more and understand how to consume and deploy apps to Kubernetes please follow [these tutorials](), which take you from deploying a single container manually through the CLI to deploying a complete application (multiple containers) via a manifest.
