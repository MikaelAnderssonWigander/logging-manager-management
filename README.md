# logging-manager-management

To reproduce

 http --form POST :8080/q/logging-manager loggerName=myapp loggerLevel=DEBUG

 This works

 Change application.yml and enable management

 quarkus.management.enabled=false

Rerun application and execute:

 http --form POST :9000/q/logging-manager loggerName=myapp loggerLevel=DEBUG

 Now it fails