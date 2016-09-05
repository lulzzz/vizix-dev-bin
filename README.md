## SETUP

1. Add bin folder to OS's PATH
2. create vizix network

    ```sh
    $ create-network
    ```

3. create data folders:

    ```sh
    $ mkdir ~/docker-volumes/mysql-data
    $ mkdir ~/docker-volumes/mongo-data
    ```

4. create basic services

    ```sh
    $ run-resolvable
    $ run-mysql
    $ run-mongo
    $ run-mosquitto
    $ run-hazelcast
    ```

5. create services

    ```sh
    $ cd <path_to_services>
    $ build-services
    $ run-services
    ```

6. create ui

    ```sh
    $ cd <path_to_ui>
    $ build-ui
    $ run-ui
    ```

## DAILY USAGE

For every day's work use build-, run- and docker start/stop as needed.
For example this could be a sequence:

```sh
$ #start basic services
$ #resolvable, mysql, mongo, mosquitto, hazelcast(s)
$ start-basic-services
$ #start services/backend
$ docker start services
$ #start ui
$ docker start ui
```
