# Инструкция по запуску Sausage Store в Kubernetes

## Запуск приложения

1. Убедитесь, что у вас установлены:
   - kubectl
   - helm

2. Установите Helm-чарт:
   ```bash
   helm install sausage-store ./sausage-store-chart
   ```

3. Проверьте, что все поды запустились:
   ```bash
   kubectl get pods
   ```

## Проверка работоспособности

1. Проверьте статус деплойментов:
   ```bash
   kubectl get deployments
   ```

2. Проверьте логи приложения:
   ```bash
   kubectl logs deployment/frontend
   kubectl logs deployment/backend
   kubectl logs deployment/backend-report
   ```

3. Проверьте сервисы и ингрессы:
   ```bash
   kubectl get svc
   kubectl get ingress
   ```

## Доступ к приложению

Фронтенд доступен по URL: http://front-movsar.2sem.students-projects.ru
