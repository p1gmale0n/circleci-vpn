# guardrailsio-circleci-vpn

CircleCI configuration:  
open `Organization Settings` -> Contexts -> kubernetes  
and configure Environment Variables:  
- **VPN_CONFIG** - base64 encoded openvpn config file.  
  To get opencpn configu - open Pritunl app, click menu button (icon with three horizontal lines) -> edit config.
- **VPN_USER** - your pritunl vpn username.
- **VPN_PASSWORD** - your pritunl vpn PIN.

*Notes:*  
This circleci job running in a dedicated, ephemeral VM.  
Using machine may require additional fees in a future pricing update.  
