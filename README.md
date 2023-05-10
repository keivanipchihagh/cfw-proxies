# cfw-proxies
Turn Cloudflare's workers into unstoppable proxies

## Why Cloudflare workers?
Cloudflare Workers provides a serverless Open external link execution environment that allows you to create new applications or augment existing ones without configuring or maintaining any infrastructure. You can use Cloudflare Workers to build entire applications that run on Cloudflare's network, deploy a global application onto 180+ data centers around the world in less than 30 seconds.


## Scripts

### v2ray.js
This script masks your V2ray address with Cloudflare Workers. It can be used to bypass the GFW easily and is accessible through all ISPs, but at the cost of a little high ping. Steps:
1. Setup V2ray on X-UI as described [here](https://github.com/keivanipchihagh/x-ui).
2. Create a new worker on [Cloudflare Workers](https://workers.cloudflare.com/).
3. Copy and modify the script `v2ray.js` to your worker. Deploy it.
4. (*Optional*) To hide your worker address, connect your Worker to a custom domain. (Can take a few hours to take effect)
5. Modify your client config by replacing the address with your worker address and your port to 443. (If you have a custom domain, use it instead of the worker address)

> **Note**
> Your V2ray config must be a **Vmess** **WebSocket**, listening on open Cloudflare ports and using **TLS**. This behavior is pretty much like CDNs.
