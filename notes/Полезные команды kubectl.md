---
Дата создания: 2025-07-02
Темы:
  - "[[Kubernetes]]"
tags:
  - "#tutorial"
---

## 📄 Работа с ресурсами

```bash
kubectl get pods                     # Список всех подов
kubectl get svc                      # Список сервисов
kubectl get deployments              # Список деплойментов
kubectl get nodes                    # Список нод кластера
kubectl get all                      # Все ресурсы в текущем namespace
```

## 🔍 Подробная информация

```bash
kubectl describe pod <name>         # Подробная инфа о поде
kubectl describe svc <name>         # Подробная инфа о сервисе
```

## 📦 Применение и удаление ресурсов

```bash
kubectl apply -f <file>.yaml        # Применить манифест
kubectl delete -f <file>.yaml       # Удалить ресурс из манифеста
kubectl delete pod <name>           # Удалить под
```

## 📂 Работа с namespace

```bash
kubectl get ns                                           # Все namespace'ы
kubectl config set-context --current --namespace=<ns>   # Сменить namespace
```

## 🐞 Отладка и логирование

```bash
kubectl logs <pod>                  # Логи пода
kubectl logs <pod> -c <container>   # Логи конкретного контейнера
kubectl exec -it <pod> -- bash      # Подключиться внутрь пода
kubectl port-forward <pod> 8080:80  # Проброс порта
```

## 🧪 Тесты и проверка

```bash
kubectl explain pod                            # Документация по ресурсу pod
kubectl rollout status deployment <name>       # Статус развёртывания
kubectl top pod                                # Использование ресурсов подами
```