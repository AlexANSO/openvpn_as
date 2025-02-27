# 文件目录结构
```
root@docker:~/docker-data/openvpn-as# tree -L 2  .
.
├── data
│   └── pyovpn-2.0-py3.10.egg  # 破解文件
└── docker-compose.yaml

1 directory, 2 files
```

# 下载对应的egg破解文件

```
wget https://github.com/AlexANSO/openvpn_as/raw/refs/heads/master/pyovpn-2.0-py3.10.egg
wget https://jsdelivr.pai233.top/gh/AlexANSO/openvpn_as@master/pyovpn-2.0-py3.10.egg  # 加速
```

# 启动docker

```
docker-compose up -d
```

# 验证配置
```
root@docker:~/docker-data/openvpn-as# docker-compose logs | grep License
openvpn-as  | OpenVPN Access Server End User License Agreement (OpenVPN-AS EULA)
openvpn-as  |     1. Copyright Notice: OpenVPN Access Server License;
openvpn-as  |        find our complete EULA (End-User License Agreement) on our website
openvpn-as  |     7. Subscription License Key: Entitles you to use this software for the
openvpn-as  |     8. Standard Non-Subscription License Key(s) also called Fixed License Key(s):
openvpn-as  | 2025-02-26T14:22:22+0000 [stdout#info] License Info {'concurrent_connections': 8888, 'apc': False}
openvpn-as  | 2025-02-26T14:22:22+0000 [stdout#info] License Info {'concurrent_connections': 8888, 'apc': False}
openvpn-as  | 2025-02-26T14:22:23+0000 [stdout#info] License Info {'concurrent_connections': 8888, 'apc': False}
openvpn-as  | 2025-02-26T14:22:23+0000 [stdout#info] License Info {'concurrent_connections': 8888, 'apc': False}
openvpn-as  | 2025-02-26T14:22:27+0000 [stdout#info] License Info {'concurrent_connections': 8888, 'apc': False}
```
<img width="1202" alt="image" src="https://github.com/user-attachments/assets/448bcc13-ad13-4cc0-80dc-f6bf242f3282" />
