zbbix_rds_monitoring
===================

AWS RDS Template for Zabbix

1. place the script "rds_stats.py" at zabbix-server externalscripts folder (/etc/zabbix/externalscripts/), make sure it has execute permission.
2. Import the template "rds_template.xml".
3. enter you aws credentials in the template's macro section ({$AWS_ACCESS_KEY},  {$AWS_SECRET_KEY}) 
4. set you default AWS region in the template's macro section {$REGION}
5. Attach the above template to the relevant hosts. The zabbix host name must match the RDS DB Instance host name
6. note that you can override the AWS region for specific hosts by adding the {$REGION} macro to the host

~                             
