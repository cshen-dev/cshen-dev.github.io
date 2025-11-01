---
layout: post
title: "🛜 Do you need a modern VPN like Tailscale?"
---

![https://upload.wikimedia.org/wikipedia/commons/thumb/4/4d/Tailscale-Logo-Black.svg/750px-Tailscale-Logo-Black.svg.png?20210201215505](https://upload.wikimedia.org/wikipedia/commons/thumb/4/4d/Tailscale-Logo-Black.svg/750px-Tailscale-Logo-Black.svg.png?20210201215505)

Virtual Private Networks (VPNs) were originally designed to let employees securely connect to their company’s internal network from anywhere. Over time, however, “VPN” has also become a consumer term, widely adopted by individuals who want to protect their online privacy by masking their IP addresses and making their activity harder to trace.

With the rise of cloud computing, on-premises servers are gradually disappearing for most businesses outside of highly regulated industries. In sectors like technology and marketing, where only a few servers remain in the office, the traditional demand for VPNs to bridge staff into the corporate network has steadily declined.


As more IT services that power business operations migrate to the cloud, securing access to those cloud assets—and the traffic between staff and applications—has become far more critical. This shift has led to the rise of Secure Access Service Edge (SASE) solutions, with Cloudflare SASE being a prime example. These services ensure that all data exchanges occur securely between verified users and provisioned cloud applications.

![https://cf-assets.www.cloudflare.com/dzlvafdwdttg/7HKAxn24Cl8po9UtqMEmYS/bf8e6b664b638e77c0a7cf59a943d3c3/Network_Connectivity_plus_Zero_Trust_Security_Diagram.svg](https://cf-assets.www.cloudflare.com/dzlvafdwdttg/7HKAxn24Cl8po9UtqMEmYS/bf8e6b664b638e77c0a7cf59a943d3c3/Network_Connectivity_plus_Zero_Trust_Security_Diagram.svg)

Does this mean VPNs have no role in a cloud-first world? Not entirely. Consider bastion hosts—long used by system administrators for privileged access. Since identity providers (IdPs) are not always integrated in such environments, a secure tunnel is often still necessary before executing sensitive commands over the public internet.

In such scenarios, modern programmable VPNs like TailScale can be a strong fit, offering affordability and a rich feature set suitable for businesses of all sizes.

That said, when we look more closely, most SaaS platforms today are hosted on major cloud providers such as AWS, GCP, and Azure. These providers already offer secure methods to access resources—for instance, AWS Session Manager can be used instead of a traditional VPN to reach bastion servers.

Over time, this trend reduces the practical need for solutions like TailScale. While TailScale is an innovative take on VPNs, its use cases are shrinking as workloads consolidate in the cloud. Unless we see a resurgence of on-premises infrastructure or more cloud-agnostic security requirements, VPN-style solutions may continue to lose relevance. Still, it’s worth revisiting this assessment regularly, as the landscape can evolve quickly.


---
**Reference**
- [Tailscale · Best VPN Service for Secure Networks](https://tailscale.com/)
- [Cloudflare vs. Tailscale - Compare Access and Gateway to Tailscale](https://tailscale.com/compare/cloudflare-access)
- [What is SASE? - Secure access service edge - Cloudflare](https://www.cloudflare.com/en-gb/learning/access-management/what-is-sase/)
- [VPN Replacement - Zero Trust - Cloudflare](https://www.cloudflare.com/en-au/zero-trust/solutions/vpn-replacement/)
- [AWS Systems Manager Session Manager - AWS Systems Manager](https://docs.aws.amazon.com/systems-manager/latest/userguide/session-manager.html)