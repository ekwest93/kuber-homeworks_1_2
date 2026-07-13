# kuber-homeworks_1_2
# Домашнее задание к занятию «Базовые объекты K8S»

### Цель задания

В тестовой среде для работы с Kubernetes, установленной в предыдущем ДЗ, необходимо развернуть Pod с приложением и подключиться к нему со своего локального компьютера. 

------

### Чеклист готовности к домашнему заданию

1. Установленное k8s-решение (например, MicroK8S).
2. Установленный локальный kubectl.
3. Редактор YAML-файлов с подключенным Git-репозиторием.

------

### Инструменты и дополнительные материалы, которые пригодятся для выполнения задания

1. Описание [Pod](https://kubernetes.io/docs/concepts/workloads/pods/) и примеры манифестов.
2. Описание [Service](https://kubernetes.io/docs/concepts/services-networking/service/).

------

### Задание 1. Создать Pod с именем hello-world

1. Создать манифест (yaml-конфигурацию) Pod.
2. Использовать image - gcr.io/kubernetes-e2e-test-images/echoserver:2.2.
3. Подключиться локально к Pod с помощью `kubectl port-forward` и вывести значение (curl или в браузере).
<img width="776" height="88" alt="image" src="https://github.com/user-attachments/assets/aa5c6ec5-dcaf-433c-991d-8de834bbeb91" />
<img width="763" height="765" alt="image" src="https://github.com/user-attachments/assets/02a10055-34ab-4cf4-9804-cb17d838ae64" />


------

### Задание 2. Создать Service и подключить его к Pod

1. Создать Pod с именем netology-web.
2. Использовать image — gcr.io/kubernetes-e2e-test-images/echoserver:2.2.
3. Создать Service с именем netology-svc и подключить к netology-web.
4. Подключиться локально к Service с помощью `kubectl port-forward` и вывести значение (curl или в браузере).
<img width="1032" height="179" alt="image" src="https://github.com/user-attachments/assets/7712cd1c-e411-4c3e-8d99-7b637c8fd379" />
   
<img width="971" height="778" alt="image" src="https://github.com/user-attachments/assets/e80ee912-12cb-4be4-b8e6-d4b750d69ba3" />


### Файлы манифестов

- [`hello-world-pod.yaml`](./hello-world-pod.yaml) — Pod для первого задания
- [`netology-web-pod.yaml`](./netology-web-pod.yaml) — Pod для второго задания
- [`netology-svc-service.yaml`](./netology-svc-service.yaml) — Service для второго задания

------

### Правила приёма работы

1. Домашняя работа оформляется в своем Git-репозитории в файле README.md. Выполненное домашнее задание пришлите ссылкой на .md-файл в вашем репозитории.
2. Файл README.md должен содержать скриншоты вывода команд `kubectl get pods`, а также скриншот результата подключения.
3. Репозиторий должен содержать файлы манифестов и ссылки на них в файле README.md.

------

### Критерии оценки
Зачёт — выполнены все задания, ответы даны в развернутой форме, приложены соответствующие скриншоты и файлы проекта, в выполненных заданиях нет противоречий и нарушения логики.

На доработку — задание выполнено частично или не выполнено, в логике выполнения заданий есть противоречия, существенные недостатки.
