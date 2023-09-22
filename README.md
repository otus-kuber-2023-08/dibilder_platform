# kubernetes-intro
1. Разобраны причины восстановления pods после удаления, описано в PR.
2. Создан Dockerfile и помещен в директорию kubernetes-intro/web
3. Создан манифест для web-pod и помещен в директорию kubernetes-intro
4. Создан исправленный манифест для frontend-pod и помещен в директорию kubernetes-intro
# kubernetes-controllers
1. Разобраны понятия Replicaset и Deployment, созданы манифесты
2. Реализованы сценарии развертывания blue-green и Reverse Rolling Update
3. Разобраны понятия Probes и Daemonset, пробы добавлены в манифесты
4. Создан DaemonSet для NodeExporter, и применен также на master ноду
# kubernetes-networks
1. Создан Deployment с Liveness и Readyness пробами и стратегией развертывания
2. Созданы Service с ClusterIP и LoadBalancer
3. Разобран балансировщик MetalLB, созданы соответствующие манифесты
4. Сделан сервис LoadBalancer, открывающий доступ к CoreDNS
5. Изучены Ingress-контроллеры, создан http-балансировщик для подов Web
6. Создан https Ingress для kubernetes-Dasboard
7. Создан Ingress для Canary подов, отправляющий 10% траффика в неймспейс Canary
