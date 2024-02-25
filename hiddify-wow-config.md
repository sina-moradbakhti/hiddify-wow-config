# hiddify-wow-config
### How to make free Warp on Warp config and use it on Hiddify to connect to the free world wide network.


# Warp on Warp

[This Config file](WoW/WarpOnWarp-HiddifyNext.json) can be used directly in the [Hiddify Next](https://github.com/hiddify/hiddify-next/releases) App. But it is better to make your personal warp config to have better speed and lower delay.

## How to make it?

### Android, Linux and Mac

1. Copy the [Config file](WoW/WarpOnWarp-HiddifyNext.json) to an editor.
2. Run the below command in the termux(Android Shell), linux or mac to acquire best working IP/Ports of the Cloudflare Warp. After running select option 1.
```
bash <(curl -fsSL https://raw.githubusercontent.com/Ptechgithub/warp/main/endip/install.sh)
```
3. Replace the two IP/Ports of the copied config file (Step 1) with one of the resulted IP/Port of the step 2.
4. Run the below instruction two times to acquire two free Warp accounts. Each time you run it, writes 3 lines including IPv6, private key and reserved bytes. You can replace the corresponding values of the copied config (Step 1) with these values.
```
curl -sL "https://api.zeroteam.top/warp?format=sing-box" | grep -Eo --color=never '"2606:4700:[0-9a-f:]+/128"|"private_key":"[0-9a-zA-Z\/+]+="|"reserved":\[[0-9]+(,[0-9]+){2}\]'
```
5. Now you can use the resulted config in the Hiddify Next App to circumvent the censorship.

### Windows

Use steps of the previous section, but:

 - Instead of step 2, Extract [this zip file](https://raw.githubusercontent.com/Elfiinaa/ConfigFiles/main/WoW/WarpIPScanner-Win-v23.11.15.zip) and open the WarpIPEndpointScanner.bat to start the scanner.
 - Instead of step 4, download and run windows version of [Warp-Reg](https://github.com/badafans/warp-reg/releases).

 ## Credits
 
 [Yonggekkk](https://github.com/yonggekkk/warp-yg) for the windows warp IP scanner

 #### If this method worked well on you, you can buy me a coffe via the following link, if you'd like, https://www.coffeebede.com/sinamoradbakhti
