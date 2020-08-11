# u2b3_platform
u2b3 Platform repository
____

# Описание проекта

## Оглавление
0. [Знакомство с Kubernetes, основные понятия и архитектура](#kubernetes-intro)

## kubernetes-intro
- настройка репоизтория
- установка и настройка kubectl & minikube (driver=none)
- запуск minikube 
- удаление namespace kube-system и всех контейнеров в docker. Мониторинг состояния и восстановления кластера kubernetes
- работа с key&value базой etcd, удаление хранилища и попытка восстановления кластера
- восстановление kubernetes из snapshot etcd хранилища
- установка dashboard
- kubectl port-forward
- k9s 
- создание Dockerfile для websrv:1.0.1, non-root container, 1001 uid. docker push to flying1900/websrv
- создание и работа с манифестом web-pod.yaml
- дополнительная настройка web-pod.yaml, добавление init контейнера и volume
- отладка работы web poda, kubectl describe & kubectl edit. Эксперименты с ошибками в манифесте
- эксперименты с [kube-forwarder](https://kube-forwarder.pixelpoint.io/)
- работа с первым frontend [HipsterShop](https://github.com/GoogleCloudPlatform/microservices-demo)
- отладка окружения frontend HipsterShop, поиск неисправностей в манифесте и эксперименты с рабочим манифестом
____
