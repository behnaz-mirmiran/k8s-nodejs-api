# k8s-nodejs-api

این پروژه یک REST API ساده نوشته‌شده با Node.js را در Kubernetes اجرا می‌کند.

## 📂 ساختار فایل‌ها

- `deployment.yaml`: اجرای Node.js API روی پاد
- `service.yaml`: ساخت سرویس NodePort برای دسترسی خارجی

## 🚀 نحوه اجرا

```bash
kubectl apply -f manifests/
## 🌐 تست پروژه

برای تست، ابتدا سرویس را اجرا کرده و سپس با دستور زیر وضعیت را بررسی کنید:

```bash
kubectl get svc node-api-service

curl http://<NodeIP>:<NodePort>
