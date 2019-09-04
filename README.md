# ansible-teamcity-build-agent

[![Build Status](https://www.travis-ci.org/miquido/ansible-teamcity-build-agent.svg?branch=master)](https://www.travis-ci.org/miquido/ansible-teamcity-build-agent)
[![License](https://img.shields.io/badge/license-MIT%20License-brightgreen.svg)](https://opensource.org/licenses/MIT)
[![Twitter URL](https://img.shields.io/twitter/follow/miquido.svg?style=social&label=Follow%20%40Miquido)](https://twitter.com/miquido)

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

## Test the role

Use your shell and put
```
molecule test
```
