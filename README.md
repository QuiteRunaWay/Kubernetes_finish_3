# Домашнее задание к занятию "14.3 Карты конфигураций"

## Задача 1: Работа с картами конфигураций через утилиту kubectl в установленном minikube

Выполните приведённые команды в консоли. Получите вывод команд. Сохраните
задачу 1 как справочный материал.

### 1.1 Как создать карту конфигураций?

```
kubectl create configmap nginx-config --from-file=nginx.conf
kubectl create configmap domain --from-literal=name=netology.ru
```
### Ответ 1.1: 

![image](https://user-images.githubusercontent.com/92969676/202639704-4903b9b1-c090-48d0-aff6-6ce7f1d950f7.png)

![image](https://user-images.githubusercontent.com/92969676/202639766-215808fc-4879-4a2a-a7f5-08ba7b5d5fb8.png)


### 1.2 Как просмотреть список карт конфигураций?

```
kubectl get configmaps
kubectl get configmap
```
### Ответ 1.2: 

![image](https://user-images.githubusercontent.com/92969676/202639847-378ee203-5a33-4e10-9beb-3290542bea31.png)


### 1.3 Как просмотреть карту конфигурации?

```
kubectl get configmap nginx-config
kubectl describe configmap domain
```
### Ответ 1.3: 

![image](https://user-images.githubusercontent.com/92969676/202639924-a1cfa22a-23a4-4666-89d9-9150abf3ef95.png)

### 1.4 Как получить информацию в формате YAML и/или JSON?

```
kubectl get configmap nginx-config -o yaml
kubectl get configmap domain -o json
```
### Ответ 1.4: 

### 1.5 Как выгрузить карту конфигурации и сохранить его в файл?

```
kubectl get configmaps -o json > configmaps.json
kubectl get configmap nginx-config -o yaml > nginx-config.yml
```
### Ответ 1.5: 

### 1.6 Как удалить карту конфигурации?

```
kubectl delete configmap nginx-config
```
### Ответ 1.6: 

### 1.7 Как загрузить карту конфигурации из файла?

```
kubectl apply -f nginx-config.yml
```
### Ответ 1.7: 
