# nginx-oracledb-healthcheck
OracleDB HTTP healthcheck in Node.JS - Integrates with Nginx

Uses Node.JS OracleDB module. Requires installations of Node.JS and OracleDB - documented here:

Oracle 21c XE - https://www.oracle.com/database/technologies/appdev/xe/quickstart.html
OracleDB Node.JS Module - https://github.com/oracle/node-oracledb
Node.JS - https://nodejs.org/en/download/package-manager/
Nginx-Plus - https://docs.nginx.com/nginx/admin-guide/installing-nginx/installing-nginx-plus/

Once the Oracle Database and NodeJS are running - add the module and associated healthcheck code. 
Nginx-Plus can then be configured to query the NodeJS healthcheck as an active HTTP check.

Example load balancing done with Nginx-Plus Active Health Check. (oracle.conf - needs include in stream context on nginx.conf)

Sample configurations provided.
