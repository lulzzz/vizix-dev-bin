## SETUP

1. Add bin folder to OS's PATH
2. create vizix network
    ```sh
    $ create-network
    ```
3. create folders:
    ```sh
    $ mkdir ~/docker-volumes/mysql-data
    $ mkdir ~/docker-volumes/mysql-data
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

1. start basic services (resolvable, mysql, mongo, mosquitto, hazelcast(s))
    ```sh
    $ start-basic-services
    ```
2. start services/backend
    ```sh
    $ docker start services
    ```
3. start ui
    ```sh
    $ docker start ui
    ```

For every day's work use build, run and docker start/stop as needed.
