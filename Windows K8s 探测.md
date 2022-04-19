# Windows K8s 探测


```
[Information Gathering - System Info]
2022/04/07 07:51:30 current dir: /
2022/04/07 07:51:30 current user: root uid: 0 gid: 0 home: /root
2022/04/07 07:51:30 hostname: nginx
2022/04/07 07:51:30 debian debian 11.3 kernel: 5.10.104-linuxkit

[Information Gathering - Services]
2022/04/07 07:51:30 sensitive env found:
        KUBERNETES_SERVICE_PORT_HTTPS=443
2022/04/07 07:51:30 sensitive env found:
        KUBERNETES_SERVICE_PORT=443
2022/04/07 07:51:30 sensitive env found:
        KUBERNETES_PORT_443_TCP=tcp://10.96.0.1:443
2022/04/07 07:51:30 sensitive env found:
        KUBERNETES_PORT_443_TCP_PROTO=tcp
2022/04/07 07:51:30 sensitive env found:
        KUBERNETES_PORT_443_TCP_ADDR=10.96.0.1
2022/04/07 07:51:30 sensitive env found:
        KUBERNETES_SERVICE_HOST=10.96.0.1
2022/04/07 07:51:30 sensitive env found:
        KUBERNETES_PORT=tcp://10.96.0.1:443
2022/04/07 07:51:30 sensitive env found:
        KUBERNETES_PORT_443_TCP_PORT=443
2022/04/07 07:51:30 service found in process:
        1       0       nginx
2022/04/07 07:51:30 service found in process:
        31      1       nginx
2022/04/07 07:51:30 service found in process:
        32      1       nginx

[Information Gathering - Commands and Capabilities]
2022/04/07 07:51:30 available commands:
        curl,wget,find,apt,dpkg,nginx,mount,base64,perl
2022/04/07 07:51:30 Capabilities hex of Caps(CapInh|CapPrm|CapEff|CapBnd|CapAmb):
        CapInh: 00000000a80425fb
        CapPrm: 00000000a80425fb
        CapEff: 00000000a80425fb
        CapBnd: 00000000a80425fb
        CapAmb: 0000000000000000
        Cap decode: 0x00000000a80425fb = CAP_CHOWN,CAP_DAC_OVERRIDE,CAP_FOWNER,CAP_FSETID,CAP_KILL,CAP_SETGID,CAP_SETUID,CAP_SETPCAP,CAP_NET_BIND_SERVICE,CAP_NET_RAW,CAP_SYS_CHROOT,CAP_MKNOD,CAP_AUDIT_WRITE,CAP_SETFCAP
        Add capability list:
[*] Maybe you can exploit the Capabilities below:

[Information Gathering - Mounts]

[Information Gathering - Net Namespace]
        container net namespace isolated.

[Information Gathering - Sysctl Variables]
2022/04/07 07:51:30 net.ipv4.conf.all.route_localnet = 0

[Discovery - K8s API Server]
2022/04/07 07:51:30 checking if api-server allows system:anonymous request.
err found in post request, error response code: 403 Forbidden.
        api-server forbids anonymous request.
        response:

[Discovery - K8s Service Account]
        service-account is available
2022/04/07 07:51:30 trying to list namespaces
err found in post request, error response code: 403 Forbidden.

[Discovery - Cloud Provider Metadata API]
2022/04/07 07:51:31 failed to dial Alibaba Cloud API.
2022/04/07 07:51:31 failed to dial Azure API.
2022/04/07 07:51:31 failed to dial Google Cloud API.
2022/04/07 07:51:32 failed to dial Tencent Cloud API.
2022/04/07 07:51:32 failed to dial OpenStack API.
2022/04/07 07:51:32 failed to dial Amazon Web Services (AWS) API.
2022/04/07 07:51:33 failed to dial ucloud API.
```
