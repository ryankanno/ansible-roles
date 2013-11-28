# javadev

This playbook installs packages / libraries associated with java development.

## playbook variables

|name|description|default|
|----|-----------|-------|
|`java.jdk.package`|java jdk package|openjdk-7-jdk|
|`java.jdk.version`|java jdk package version|7u25-2.3.10-1ubuntu0.12.10.2|
|`java.sdk.package`|java sdk package||
|`java.sdk.version`|java sdk package version||
|`java.libraries.latest`|latest java packages to install||
|`java.libraries.versioned`|versioned java packages to install||

See [defaults/main.yml](https://github.com/ryankanno/playbooks/blob/master/javadev/defaults/main.yml)
