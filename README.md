## Creación del paquete Helm y publicación

Para empaquetar el chart y colocarlo en el directorio de publicación (`./docs/`), ejecuta el siguiente comando:

```bash
helm package chart-backend-enterprise-aws/ --destination ./docs/

```
Crar index para que permita el descargue del charts
```bash
helm repo index docs/ --url https://mct-desarrollo.github.io/helm-charts/

```

Este comando genera un archivo .tgz dentro del folder docs/, el cual puede ser utilizado como parte de un repositorio Helm estático.