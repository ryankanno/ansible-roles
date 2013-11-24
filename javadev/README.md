# javadev

This playbook installs packages / libraries associated with java development.

## playbook variables

|name|description|default|
|----|-----------|-------|
|`java.jdk.package`|java jdk package|openjdk-7-jdk|
|`java.jdk.version`|python package version|7u25-2.3.10-1ubuntu0.12.10.2|
|`java.sdk.package`|python package||
|`java.sdk.version`|python package version||
|`java.libraries.latest`|latest java packages to install||
|`java.libraries.versioned`|versioned java packages to install||

See [defaults/main.yml](https://github.com/ryankanno/playbooks/blob/master/javadev/defaults/main.yml)
