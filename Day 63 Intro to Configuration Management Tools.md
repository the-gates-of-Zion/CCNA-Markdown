# Intro to Configuration Management Tools

## Tools avalible

### Ansible

- python

- agentless

	- doesn't require any special software to run on managed devices

	- management device --ssh-> devices

- ssh connect to devices

	- make configuration changes

	- extract information

- Push model

	- Sever push to devices

- create text files

	- Playbooks

		- outline the logic and actions of the tasks that ansible should do

	- inventory files

	- Templates

### Puppet

- pull model

- Ruby

- Agent-based

	- Specific software must be installed on the managed device

- uses TCP 8140 to communicate with master

### Chef

- pull model

- Written in Ruby

- Not all Cisco support a chef agent

- TCP 10002 to send configurations to clients

## Configuration Drift

### Individual changes made over time

- deviate from the standard configurations as defined by the company

### Device's config is usually defined in standard templates designed by the network architects of the company

- large scale

- check fo compliance with defined standards

### without automation tools

- images

- uses standard naming system

- Correct config is not necessary is the latest config

- does not scale

## Configuration Provisioning

### how config changes are applied to devices

