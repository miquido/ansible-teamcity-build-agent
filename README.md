# ansible-teamcity-build-agent

## Synopsis

Installing and configuring a TeamCity agent.

## Requirements

You need to have installed Java.

## Variables

Protocol using to connect with TeamCity server:
```
teamcity_agent_server_url_protocol: http
```

TeamCity server address:
```
teamcity_agent_server_url: localhost
```

TeamCity build agent install directory:
```
teamcity_agent_install_dir: /opt/buildAgent
```

TeamCity administrator user:
```
teamcity_server_user_name: teamcity
```

TeamCity administrator password:
```
teamcity_server_user_passwd: teamcity
```

## Usage

```
---

- hosts: all
  become: yes
  roles:
    - ansible-teamcity-build-agent
```
