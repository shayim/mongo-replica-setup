# Steps to setup mongo replica for local development

1.  [Medium tutorial by Prasanth Kanikicherla](https://prashix.medium.com/setup-mongodb-replicaset-with-authentication-enabled-using-docker-compose-5edd2ad46a90)

2.  ```
    chmod 400 file.key
    chmod +x setup.sh
    ```

3.  edit /etc/hosts - add mongo replica set hostname

    ```
    127.0.0.1 mongo-1.mongo mongo-2.mongo mongo-3.mongo
    ```

4.  Connection String
    ```
    mongodb://admin:password@mongo-1.mongo,mongo-2.mongo,mongo-3.mongo/?replicaSet=rs
    ```
