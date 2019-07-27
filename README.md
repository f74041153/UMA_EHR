## What is it?
`UMA_EHR` is a project modified from `keycloak-quickstarts`. 
It demonstrates a simplified way to exchange health record based on UMA framework.
## Notice
Please place the whole directory "UMA_EHR" under "keycloak-quickstarts" as the same level of "app-authz-uma-photoz".That is
```
keycloak-quickstarts
|_ app-authz-uma-photoz
|_ UMA_EHR
```

## Role
* **EHR-html5-client** : 3rd party app
* **HP1** : Hospital, Resource Server1
* **HP2** : Hospital, Resource Server2
* **Keycloak** : Authorization Server

## User for demo
ID,PWD :
* alice,alice
* jdoe,jdoe
* admin,admin

## Deploy and Run
### HP1
```
cd HP1
mvn clean package wildfly:deploy
```
### HP2
```
cd HP2
mvn clean package wildfly:deploy
```
### EHR-html5-client
```
$ cd photoz-html5-client
$ mvn clean wildfly:deploy
```
Then access 
`http://localhost:8080/EHR-html5-client`

## Demo 
https://hackmd.io/@83VCk1VZSiCVJJdX97QEMg/SJMHrWfC4#/3/1
press down arrow key to see more details
