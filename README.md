<!-- DO NOT EDIT THIS FILE MANUALLY -->
<!-- Please read https://github.com/linuxserver/docker-wireguard/blob/legacy/.github/CONTRIBUTING.md -->
[![linuxserver.io](https://raw.githubusercontent.com/linuxserver/docker-templates/master/linuxserver.io/img/linuxserver_medium.png)](https://linuxserver.io)

[![Blog](https://img.shields.io/static/v1.svg?color=94398d&labelColor=555555&logoColor=ffffff&style=for-the-badge&label=linuxserver.io&message=Blog)](https://blog.linuxserver.io "all the things you can do with our containers including How-To guides, opinions and much more!")
[![Discord](https://img.shields.io/discord/354974912613449730.svg?color=94398d&labelColor=555555&logoColor=ffffff&style=for-the-badge&label=Discord&logo=discord)](https://discord.gg/YWrKVTn "realtime support / chat with the community and the team.")
[![Discourse](https://img.shields.io/discourse/https/discourse.linuxserver.io/topics.svg?color=94398d&labelColor=555555&logoColor=ffffff&style=for-the-badge&logo=discourse)](https://discourse.linuxserver.io "post on our community forum.")
[![Fleet](https://img.shields.io/static/v1.svg?color=94398d&labelColor=555555&logoColor=ffffff&style=for-the-badge&label=linuxserver.io&message=Fleet)](https://fleet.linuxserver.io "an online web interface which displays all of our maintained images.")
[![GitHub](https://img.shields.io/static/v1.svg?color=94398d&labelColor=555555&logoColor=ffffff&style=for-the-badge&label=linuxserver.io&message=GitHub&logo=github)](https://github.com/linuxserver "view the source for all of our repositories.")
[![Open Collective](https://img.shields.io/opencollective/all/linuxserver.svg?color=94398d&labelColor=555555&logoColor=ffffff&style=for-the-badge&label=Supporters&logo=open%20collective)](https://opencollective.com/linuxserver "please consider helping us by either donating or contributing to our budget")

The [LinuxServer.io](https://linuxserver.io) team brings you another container release featuring:

* regular and timely application updates
* easy user mappings (PGID, PUID)
* custom base image with s6 overlay
* weekly base OS updates with common layers across the entire LinuxServer.io ecosystem to minimise space usage, down time and bandwidth
* regular security updates

Find us at:

* [Blog](https://blog.linuxserver.io) - all the things you can do with our containers including How-To guides, opinions and much more!
* [Discord](https://discord.gg/YWrKVTn) - realtime support / chat with the community and the team.
* [Discourse](https://discourse.linuxserver.io) - post on our community forum.
* [Fleet](https://fleet.linuxserver.io) - an online web interface which displays all of our maintained images.
* [GitHub](https://github.com/linuxserver) - view the source for all of our repositories.
* [Open Collective](https://opencollective.com/linuxserver) - please consider helping us by either donating or contributing to our budget

# [linuxserver/wireguard](https://github.com/linuxserver/docker-wireguard)

[![Scarf.io pulls](https://scarf.sh/installs-badge/linuxserver-ci/linuxserver%2Fwireguard?color=94398d&label-color=555555&logo-color=ffffff&style=for-the-badge&package-type=docker)](https://scarf.sh/gateway/linuxserver-ci/docker/linuxserver%2Fwireguard)
[![GitHub Stars](https://img.shields.io/github/stars/linuxserver/docker-wireguard.svg?color=94398d&labelColor=555555&logoColor=ffffff&style=for-the-badge&logo=github)](https://github.com/linuxserver/docker-wireguard)
[![GitHub Release](https://img.shields.io/github/release/linuxserver/docker-wireguard.svg?color=94398d&labelColor=555555&logoColor=ffffff&style=for-the-badge&logo=github)](https://github.com/linuxserver/docker-wireguard/releases)
[![GitHub Package Repository](https://img.shields.io/static/v1.svg?color=94398d&labelColor=555555&logoColor=ffffff&style=for-the-badge&label=linuxserver.io&message=GitHub%20Package&logo=github)](https://github.com/linuxserver/docker-wireguard/packages)
[![GitLab Container Registry](https://img.shields.io/static/v1.svg?color=94398d&labelColor=555555&logoColor=ffffff&style=for-the-badge&label=linuxserver.io&message=GitLab%20Registry&logo=gitlab)](https://gitlab.com/linuxserver.io/docker-wireguard/container_registry)
[![Quay.io](https://img.shields.io/static/v1.svg?color=94398d&labelColor=555555&logoColor=ffffff&style=for-the-badge&label=linuxserver.io&message=Quay.io)](https://quay.io/repository/linuxserver.io/wireguard)
[![Docker Pulls](https://img.shields.io/docker/pulls/linuxserver/wireguard.svg?color=94398d&labelColor=555555&logoColor=ffffff&style=for-the-badge&label=pulls&logo=docker)](https://hub.docker.com/r/linuxserver/wireguard)
[![Docker Stars](https://img.shields.io/docker/stars/linuxserver/wireguard.svg?color=94398d&labelColor=555555&logoColor=ffffff&style=for-the-badge&label=stars&logo=docker)](https://hub.docker.com/r/linuxserver/wireguard)
[![Jenkins Build](https://img.shields.io/jenkins/build?labelColor=555555&logoColor=ffffff&style=for-the-badge&jobUrl=https%3A%2F%2Fci.linuxserver.io%2Fjob%2FDocker-Pipeline-Builders%2Fjob%2Fdocker-wireguard%2Fjob%2Flegacy%2F&logo=jenkins)](https://ci.linuxserver.io/job/Docker-Pipeline-Builders/job/docker-wireguard/job/legacy/)

[WireGuard®](https://www.wireguard.com/) is an extremely simple yet fast and modern VPN that utilizes state-of-the-art cryptography. It aims to be faster, simpler, leaner, and more useful than IPsec, while avoiding the massive headache. It intends to be considerably more performant than OpenVPN. WireGuard is designed as a general purpose VPN for running on embedded interfaces and super computers alike, fit for many different circumstances. Initially released for the Linux kernel, it is now cross-platform (Windows, macOS, BSD, iOS, Android) and widely deployable. It is currently under heavy development, but already it might be regarded as the most secure, easiest to use, and simplest VPN solution in the industry.

[![wireguard](https://www.wireguard.com/img/wireguard.svg)](https://www.wireguard.com/)

## Supported Architectures

We utilise the docker manifest for multi-platform awareness. More information is available from docker [here](https://distribution.github.io/distribution/spec/manifest-v2-2/#manifest-list) and our announcement [here](https://blog.linuxserver.io/2019/02/21/the-lsio-pipeline-project/).

Simply pulling `lscr.io/linuxserver/wireguard:legacy` should retrieve the correct image for your arch, but you can also pull specific arch images via tags.

The architectures supported by this image are:

| Architecture | Available | Tag |
| :----: | :----: | ---- |
| x86-64 | ✅ | amd64-\<version tag\> |
| arm64 | ✅ | arm64v8-\<version tag\> |
| armhf | ❌ | |

## Version Tags

This image provides various versions that are available via tags. Please read the descriptions carefully and exercise caution when using unstable or development tags.

| Tag | Available | Description |
| :----: | :----: |--- |
| latest | ✅ | Stable releases based on Alpine *without* support for compiling Wireguard modules. |
| legacy | ✅ | Stable releases with support for compiling Wireguard modules for older kernels. |

## Application Setup

During container start, it will first check if the wireguard module is already installed and loaded. Kernels newer than 5.6 generally have the wireguard module built-in (along with some older custom kernels). However, the module may not be enabled. Make sure it is enabled prior to starting the container.

If the kernel is not built-in, or installed on host, the container will check if the kernel headers are present (in `/usr/src`) and if not, it will attempt to download the necessary kernel headers from the `ubuntu xenial/bionic`, `debian/raspbian buster` repos; then will attempt to compile and install the kernel module. If the kernel headers are not found in either `usr/src` or in the repos mentioned, container will sleep indefinitely as wireguard cannot be installed.

If you're on a debian/ubuntu based host with a custom or downstream distro provided kernel (ie. Pop!_OS), the container won't be able to install the kernel headers from the regular ubuntu and debian repos. In those cases, you can try installing the headers on the host via `sudo apt install linux-headers-$(uname -r)` (if distro version) and then add a volume mapping for `/usr/src:/usr/src`, or if custom built, map the location of the existing headers to allow the container to use host installed headers to build the kernel module (tested successful on Pop!_OS, ymmv).

With regards to arm32/64 devices, Raspberry Pi 2-4 running the [official ubuntu images](https://ubuntu.com/download/raspberry-pi) or Raspbian Buster are supported out of the box. For all other devices and OSes, you can try installing the kernel headers on the host, and mapping `/usr/src:/usr/src` and it may just work (no guarantees).

This can be run as a server or a client, based on the parameters used.

## Server Mode

If the environment variable `PEERS` is set to a number or a list of strings separated by comma, the container will run in server mode and the necessary server and peer/client confs will be generated. The peer/client config qr codes will be output in the docker log if `LOG_CONFS` is set to `true`. They will also be saved in text and png format under `/config/peerX` in case `PEERS` is a variable and an integer or `/config/peer_X` in case a list of names was provided instead of an integer.

Variables `SERVERURL`, `SERVERPORT`, `INTERNAL_SUBNET`, `PEERDNS`, `INTERFACE`, `ALLOWEDIPS` and `PERSISTENTKEEPALIVE_PEERS` are optional variables used for server mode. Any changes to these environment variables will trigger regeneration of server and peer confs. Peer/client confs will be recreated with existing private/public keys. Delete the peer folders for the keys to be recreated along with the confs.

To add more peers/clients later on, you increment the `PEERS` environment variable or add more elements to the list and recreate the container.

To display the QR codes of active peers again, you can use the following command and list the peer numbers as arguments: `docker exec -it wireguard /app/show-peer 1 4 5` or `docker exec -it wireguard /app/show-peer myPC myPhone myTablet` (Keep in mind that the QR codes are also stored as PNGs in the config folder).

The templates used for server and peer confs are saved under `/config/templates`. Advanced users can modify these templates and force conf generation by deleting `/config/wg_confs/wg0.conf` and restarting the container.

The container managed server conf is hardcoded to `wg0.conf`. However, the users can add additional tunnel config files with `.conf` extensions into `/config/wg_confs/` and the container will attempt to start them all in alphabetical order. If any one of the tunnels fail, they will all be stopped and the default route will be deleted, requiring user intervention to fix the invalid conf and a container restart.

## Client Mode

Do not set the `PEERS` environment variable. Drop your client conf(s) into the config folder as `/config/wg_confs/<tunnel name>.conf` and start the container. If there are multiple tunnel configs, the container will attempt to start them all in alphabetical order. If any one of the tunnels fail, they will all be stopped and the default route will be deleted, requiring user intervention to fix the invalid conf and a container restart.

If you get IPv6 related errors in the log and connection cannot be established, edit the `AllowedIPs` line in your peer/client wg0.conf to include only `0.0.0.0/0` and not `::/0`; and restart the container.

## Road warriors, roaming and returning home

If you plan to use Wireguard both remotely and locally, say on your mobile phone, you will need to consider routing. Most firewalls will not route ports forwarded on your WAN interface correctly to the LAN out of the box. This means that when you return home, even though you can see the Wireguard server, the return packets will probably get lost.

This is not a Wireguard specific issue and the two generally accepted solutions are NAT reflection (setting your edge router/firewall up in such a way as it translates internal packets correctly) or split horizon DNS (setting your internal DNS to return the private rather than public IP when connecting locally).

Both of these approaches have positives and negatives however their setup is out of scope for this document as everyone's network layout and equipment will be different.

## Maintaining local access to attached services

** Note: This is not a supported configuration by Linuxserver.io - use at your own risk.

When routing via Wireguard from another container using the `service` option in docker, you might lose access to the containers webUI locally. To avoid this, exclude the docker subnet from being routed via Wireguard by modifying your `wg0.conf` like so (modifying the subnets as you require):

  ```ini
  [Interface]
  PrivateKey = <private key>
  Address = 9.8.7.6/32
  DNS = 8.8.8.8
  PostUp = DROUTE=$(ip route | grep default | awk '{print $3}'); HOMENET=192.168.0.0/16; HOMENET2=10.0.0.0/8; HOMENET3=172.16.0.0/12; ip route add $HOMENET3 via $DROUTE;ip route add $HOMENET2 via $DROUTE; ip route add $HOMENET via $DROUTE;iptables -I OUTPUT -d $HOMENET -j ACCEPT;iptables -A OUTPUT -d $HOMENET2 -j ACCEPT; iptables -A OUTPUT -d $HOMENET3 -j ACCEPT;  iptables -A OUTPUT ! -o %i -m mark ! --mark $(wg show %i fwmark) -m addrtype ! --dst-type LOCAL -j REJECT
  PreDown = HOMENET=192.168.0.0/16; HOMENET2=10.0.0.0/8; HOMENET3=172.16.0.0/12; ip route del $HOMENET3 via $DROUTE;ip route del $HOMENET2 via $DROUTE; ip route del $HOMENET via $DROUTE; iptables -D OUTPUT ! -o %i -m mark ! --mark $(wg show %i fwmark) -m addrtype ! --dst-type LOCAL -j REJECT; iptables -D OUTPUT -d $HOMENET -j ACCEPT; iptables -D OUTPUT -d $HOMENET2 -j ACCEPT; iptables -D OUTPUT -d $HOMENET3 -j ACCEPT
  ```

## Site-to-site VPN

** Note: This is not a supported configuration by Linuxserver.io - use at your own risk.

Site-to-site VPN in server mode requires customizing the `AllowedIPs` statement for a specific peer in `wg0.conf`. Since `wg0.conf` is autogenerated when server vars are changed, it is not recommended to edit it manually.

In order to customize the `AllowedIPs` statement for a specific peer in `wg0.conf`, you can set an env var `SERVER_ALLOWEDIPS_PEER_<peer name or number>` to the additional subnets you'd like to add, comma separated and excluding the peer IP (ie. `"192.168.1.0/24,192.168.2.0/24"`). Replace `<peer name or number>` with either the name or number of a peer (whichever is used in the `PEERS` var).

For instance `SERVER_ALLOWEDIPS_PEER_laptop="192.168.1.0/24,192.168.2.0/24"` will result in the wg0.conf entry `AllowedIPs = 10.13.13.2,192.168.1.0/24,192.168.2.0/24` for the peer named `laptop`.

Keep in mind that this var will only be considered when the confs are regenerated. Adding this var for an existing peer won't force a regeneration. You can delete wg0.conf and restart the container to force regeneration if necessary.

Don't forget to set the necessary POSTUP and POSTDOWN rules in your client's peer conf for lan access.

## Usage

To help you get started creating a container from this image you can either use docker-compose or the docker cli.

### docker-compose (recommended, [click here for more info](https://docs.linuxserver.io/general/docker-compose))

```yaml
---
services:
  wireguard:
    image: lscr.io/linuxserver/wireguard:legacy
    container_name: wireguard
    cap_add:
      - NET_ADMIN
      - SYS_MODULE
    environment:
      - PUID=1000
      - PGID=1000
      - TZ=Etc/UTC
      - SERVERURL=wireguard.domain.com #optional
      - SERVERPORT=51820 #optional
      - PEERS=1 #optional
      - PEERDNS=auto #optional
      - INTERNAL_SUBNET=10.13.13.0 #optional
      - ALLOWEDIPS=0.0.0.0/0 #optional
      - PERSISTENTKEEPALIVE_PEERS= #optional
      - LOG_CONFS=true #optional
    volumes:
      - /path/to/appdata/config:/config
      - /lib/modules:/lib/modules #optional
    ports:
      - 51820:51820/udp
    sysctls:
      - net.ipv4.conf.all.src_valid_mark=1
    restart: unless-stopped
```

### docker cli ([click here for more info](https://docs.docker.com/engine/reference/commandline/cli/))

```bash
docker run -d \
  --name=wireguard \
  --cap-add=NET_ADMIN \
  --cap-add=SYS_MODULE \
  -e PUID=1000 \
  -e PGID=1000 \
  -e TZ=Etc/UTC \
  -e SERVERURL=wireguard.domain.com `#optional` \
  -e SERVERPORT=51820 `#optional` \
  -e PEERS=1 `#optional` \
  -e PEERDNS=auto `#optional` \
  -e INTERNAL_SUBNET=10.13.13.0 `#optional` \
  -e ALLOWEDIPS=0.0.0.0/0 `#optional` \
  -e PERSISTENTKEEPALIVE_PEERS= `#optional` \
  -e LOG_CONFS=true `#optional` \
  -p 51820:51820/udp \
  -v /path/to/appdata/config:/config \
  -v /lib/modules:/lib/modules `#optional` \
  --sysctl="net.ipv4.conf.all.src_valid_mark=1" \
  --restart unless-stopped \
  lscr.io/linuxserver/wireguard:legacy
```

## Parameters

Containers are configured using parameters passed at runtime (such as those above). These parameters are separated by a colon and indicate `<external>:<internal>` respectively. For example, `-p 8080:80` would expose port `80` from inside the container to be accessible from the host's IP on port `8080` outside the container.

| Parameter | Function |
| :----: | --- |
| `-p 51820/udp` | wireguard port |
| `-e PUID=1000` | for UserID - see below for explanation |
| `-e PGID=1000` | for GroupID - see below for explanation |
| `-e TZ=Etc/UTC` | specify a timezone to use, see this [list](https://en.wikipedia.org/wiki/List_of_tz_database_time_zones#List). |
| `-e SERVERURL=wireguard.domain.com` | External IP or domain name for docker host. Used in server mode. If set to `auto`, the container will try to determine and set the external IP automatically |
| `-e SERVERPORT=51820` | External port for docker host. Used in server mode. |
| `-e PEERS=1` | Number of peers to create confs for. Required for server mode. Can also be a list of names: `myPC,myPhone,myTablet` (alphanumeric only) |
| `-e PEERDNS=auto` | DNS server set in peer/client configs (can be set as `8.8.8.8`). Used in server mode. Defaults to `auto`, which uses wireguard docker host's DNS via included CoreDNS forward. |
| `-e INTERNAL_SUBNET=10.13.13.0` | Internal subnet for the wireguard and server and peers (only change if it clashes). Used in server mode. |
| `-e ALLOWEDIPS=0.0.0.0/0` | The IPs/Ranges that the peers will be able to reach using the VPN connection. If not specified the default value is: '0.0.0.0/0, ::0/0' This will cause ALL traffic to route through the VPN, if you want split tunneling, set this to only the IPs you would like to use the tunnel AND the ip of the server's WG ip, such as 10.13.13.1. |
| `-e PERSISTENTKEEPALIVE_PEERS=` | Set to `all` or a list of comma separated peers (ie. `1,4,laptop`) for the wireguard server to send keepalive packets to listed peers every 25 seconds. Useful if server is accessed via domain name and has dynamic IP. Used only in server mode. |
| `-e LOG_CONFS=true` | Generated QR codes will be displayed in the docker log. Set to `false` to skip log output. |
| `-v /config` | Contains all relevant configuration files. |
| `-v /lib/modules` | Maps host's modules folder. Only required if compiling wireguard modules. |
| `--sysctl=` | Required for client mode. |

### Portainer notice

This image utilises `cap_add` or `sysctl` to work properly. This is not implemented properly in some versions of Portainer, thus this image may not work if deployed through Portainer.

## Environment variables from files (Docker secrets)

You can set any environment variable from a file by using a special prepend `FILE__`.

As an example:

```bash
-e FILE__MYVAR=/run/secrets/mysecretvariable
```

Will set the environment variable `MYVAR` based on the contents of the `/run/secrets/mysecretvariable` file.

## Umask for running applications

For all of our images we provide the ability to override the default umask settings for services started within the containers using the optional `-e UMASK=022` setting.
Keep in mind umask is not chmod it subtracts from permissions based on it's value it does not add. Please read up [here](https://en.wikipedia.org/wiki/Umask) before asking for support.

## User / Group Identifiers

When using volumes (`-v` flags), permissions issues can arise between the host OS and the container, we avoid this issue by allowing you to specify the user `PUID` and group `PGID`.

Ensure any volume directories on the host are owned by the same user you specify and any permissions issues will vanish like magic.

In this instance `PUID=1000` and `PGID=1000`, to find yours use `id your_user` as below:

```bash
id your_user
```

Example output:

```text
uid=1000(your_user) gid=1000(your_user) groups=1000(your_user)
```

## Docker Mods

[![Docker Mods](https://img.shields.io/badge/dynamic/yaml?color=94398d&labelColor=555555&logoColor=ffffff&style=for-the-badge&label=wireguard&query=%24.mods%5B%27wireguard%27%5D.mod_count&url=https%3A%2F%2Fraw.githubusercontent.com%2Flinuxserver%2Fdocker-mods%2Fmaster%2Fmod-list.yml)](https://mods.linuxserver.io/?mod=wireguard "view available mods for this container.") [![Docker Universal Mods](https://img.shields.io/badge/dynamic/yaml?color=94398d&labelColor=555555&logoColor=ffffff&style=for-the-badge&label=universal&query=%24.mods%5B%27universal%27%5D.mod_count&url=https%3A%2F%2Fraw.githubusercontent.com%2Flinuxserver%2Fdocker-mods%2Fmaster%2Fmod-list.yml)](https://mods.linuxserver.io/?mod=universal "view available universal mods.")

We publish various [Docker Mods](https://github.com/linuxserver/docker-mods) to enable additional functionality within the containers. The list of Mods available for this image (if any) as well as universal mods that can be applied to any one of our images can be accessed via the dynamic badges above.

## Support Info

* Shell access whilst the container is running:

    ```bash
    docker exec -it wireguard /bin/bash
    ```

* To monitor the logs of the container in realtime:

    ```bash
    docker logs -f wireguard
    ```

* Container version number:

    ```bash
    docker inspect -f '{{ index .Config.Labels "build_version" }}' wireguard
    ```

* Image version number:

    ```bash
    docker inspect -f '{{ index .Config.Labels "build_version" }}' lscr.io/linuxserver/wireguard:legacy
    ```

## Updating Info

Most of our images are static, versioned, and require an image update and container recreation to update the app inside. With some exceptions (noted in the relevant readme.md), we do not recommend or support updating apps inside the container. Please consult the [Application Setup](#application-setup) section above to see if it is recommended for the image.

Below are the instructions for updating containers:

### Via Docker Compose

* Update images:
    * All images:

        ```bash
        docker-compose pull
        ```

    * Single image:

        ```bash
        docker-compose pull wireguard
        ```

* Update containers:
    * All containers:

        ```bash
        docker-compose up -d
        ```

    * Single container:

        ```bash
        docker-compose up -d wireguard
        ```

* You can also remove the old dangling images:

    ```bash
    docker image prune
    ```

### Via Docker Run

* Update the image:

    ```bash
    docker pull lscr.io/linuxserver/wireguard:legacy
    ```

* Stop the running container:

    ```bash
    docker stop wireguard
    ```

* Delete the container:

    ```bash
    docker rm wireguard
    ```

* Recreate a new container with the same docker run parameters as instructed above (if mapped correctly to a host folder, your `/config` folder and settings will be preserved)
* You can also remove the old dangling images:

    ```bash
    docker image prune
    ```

### Image Update Notifications - Diun (Docker Image Update Notifier)

**tip**: We recommend [Diun](https://crazymax.dev/diun/) for update notifications. Other tools that automatically update containers unattended are not recommended or supported.

## Building locally

If you want to make local modifications to these images for development purposes or just to customize the logic:

```bash
git clone https://github.com/linuxserver/docker-wireguard.git
cd docker-wireguard
docker build \
  --no-cache \
  --pull \
  -t lscr.io/linuxserver/wireguard:legacy .
```

The ARM variants can be built on x86_64 hardware using `multiarch/qemu-user-static`

```bash
docker run --rm --privileged multiarch/qemu-user-static:register --reset
```

Once registered you can define the dockerfile to use with `-f Dockerfile.aarch64`.

## Versions

* **03.10.23:** - **Potentially Breaking Change:** Support for multiple interfaces added. Wireguard confs moved to `/config/wg_confs/`. Any file with a `.conf` extension in that folder will be treated as a live tunnel config and will be attempted to start. If any of the tunnels fail, all tunnels will be stopped. Tunnels are started in alphabetical order. Managed server conf will continue to be hardcoded to `wg0.conf`.
* **24.06.23:** - Deprecate armhf as per [https://www.linuxserver.io/armhf](https://www.linuxserver.io/armhf).
* **26.04.23:** - Rework branches, swap alpine & ubuntu builds.
* **28.01.23:** - Patch wg-quick to suppress false positive sysctl warning.
* **10.01.23:** - Add new var to add `PersistentKeepalive` to server config for select peers to survive server IP changes when domain name is used.
* **26.10.22:** - Better handle unsupported peer names. Improve logging.
* **12.10.22:** - Add Alpine branch. Optimize wg and coredns services.
* **09.10.22:** - Switch back to iptables-legacy due to issues on some hosts.
* **04.10.22:** - Rebase to Jammy. Upgrade to s6v3.
* **16.05.22:** - Improve NAT handling in server mode when multiple ethernet devices are present.
* **23.04.22:** - Add pre-shared key support. Automatically added to all new peer confs generated, existing ones are left without to ensure no breaking changes.
* **10.04.22:** - Rebase to Ubuntu Focal. Add `LOG_CONFS` env var. Remove deprecated `add-peer` command.
* **28.10.21:** - Add site-to-site vpn support.
* **11.02.21:** - Fix bug related to changing internal subnet and named peer confs not updating.
* **06.10.20:** - Disable CoreDNS in client mode, or if port 53 is already in use in server mode.
* **04.10.20:** - Allow to specify a list of names as PEERS and add ALLOWEDIPS environment variable. Also, add peer name/id to each one of the peer sections in wg0.conf. Important: Existing users need to delete `/config/templates/peer.conf` and restart
* **27.09.20:** - Cleaning service binding example to have accurate PreDown script.
* **06.08.20:** - Replace resolvconf with openresolv due to dns issues when a client based on this image is connected to a server also based on this image. Add IPv6 info to readme. Display kernel version in logs.
* **29.07.20:** - Update Coredns config to detect dns loops (existing users need to delete `/config/coredns/Corefile` and restart).
* **27.07.20:** - Update Coredns config to prevent issues with non-user-defined bridge networks (existing users need to delete `/config/coredns/Corefile` and restart).
* **05.07.20:** - Add Debian updates and security repos for headers.
* **25.06.20:** - Simplify module tests, prevent iptables issues from resulting in false negatives.
* **19.06.20:** - Add support for Ubuntu Focal (20.04) kernels. Compile wireguard tools and kernel module instead of using the ubuntu packages. Make module install optional. Improve verbosity in logs.
* **29.05.20:** - Add support for 64bit raspbian.
* **28.04.20:** - Add Buster/Stretch backports repos for Debian. Tested with OMV 5 and OMV 4 (on kernel 4.19.0-0.bpo.8-amd64).
* **20.04.20:** - Fix typo in client mode conf existence check.
* **13.04.20:** - Fix bug that forced conf recreation on every start.
* **08.04.20:** - Add arm32/64 builds and enable multi-arch (rpi4 with ubuntu and raspbian buster tested). Add CoreDNS for `PEERDNS=auto` setting. Update the `add-peer`/`show-peer` scripts to utilize the templates and the `INTERNAL_SUBNET` var (previously missed, oops).
* **05.04.20:** - Add `INTERNAL_SUBNET` variable to prevent subnet clashes. Add templates for server and peer confs.
* **01.04.20:** - Add `show-peer` script and include info on host installed headers.
* **31.03.20:** - Initial Release.
