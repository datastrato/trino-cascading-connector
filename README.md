# Trino Plugin

This project is licensed under the Server Side Public License (SSPL), v 1. See the [LICENSE](./LICENSE) file for details.

This is a plugin for Trino that allows you to query data from anther Trino cluster. 

Notice tha it only supports the SELECT queries.

## License
This project is licensed under the Server Side Public License, v 1. You may not use this file except in compliance with the License. You may obtain a copy of the License at:

https://www.mongodb.com/licensing/server-side-public-license

## Build
Build the plugin with the following command:

```bash
mvn package -DskipTests
```


## Connection Confiuration
Create new properties file like <catalog-name>.properties inside etc/catalog dir:

```text
connector.name=trino
connection-url=jdbc:trino://ip:port
connection-user=myuser
connection-password=mypassword
```
