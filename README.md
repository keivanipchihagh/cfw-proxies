# cfw-proxies
Turn Cloudflare's workers into unstoppable proxies

## Scripts
### v2ray.js
This script masks your V2ray address with Cloudflare Workers. It can be used to bypass the GFW easily and is accessible through all ISPs, but at the cost of high ping. Steps:
1. Setup V2ray as described [here](https://github.com/keivanipchihagh/x-ui).
2. Create a new worker on [Cloudflare Workers](https://workers.cloudflare.com/).
3. Copy and modify the script `v2ray.js` to your worker. Deploy it.
4. (*Optional*) To hide your worker address, connect your Worker to a custom domain. (Can take a few hours to take effect)