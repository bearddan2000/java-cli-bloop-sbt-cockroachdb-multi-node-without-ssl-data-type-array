# java-cli-bloop-sbt-cockroachdb-multi-node-without-ssl-data-type-array

## Description
Creates a small table `dog` that uses
a text array data type. Arrays can also be
numeric.

A java bloop-sbt build, that connects to 3 node cluster
cockroach database without ssl.

Compiled and ran from build server `bloop`.

# Build note
Dependencies must be compatable with jdk8 or less.

## Tech stack
- bloop
- java
- bloop-sbt
  - postgres drivers

## Docker stack
- cockroachdb/cockroach:v19.2.2
- hseeberger/scala-bloop-sbt:11.0.2-oraclelinux7_1.3.5_2.12.10

## To run
`sudo ./install.sh -u`
- [Master node webui](http://localhost:8000)
- [Slave node 1 webui](http://localhost:8001)
- [Slave node 2 webui](http://localhost:8002)

## To stop
`sudo ./install.sh -d`

## For help
`sudo ./install.sh -h`

## Credit
[Cockroach setup](https://github.com/s0rg/cockroach-compose)
