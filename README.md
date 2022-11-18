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

### 1.2 Как просмотреть список карт конфигураций?

```
kubectl get configmaps
kubectl get configmap
```
### Ответ 1.2: 

### 1.3 Как просмотреть карту конфигурации?

```
kubectl get configmap nginx-config
kubectl describe configmap domain
```
### Ответ 1.3: 

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
