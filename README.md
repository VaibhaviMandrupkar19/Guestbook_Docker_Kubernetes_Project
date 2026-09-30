# Guestbook — Docker and Kubernetes Final Project

This starter project includes the application HTML, Dockerfile, and Kubernetes Deployment/Service manifest.

## Files
- `index.html` — default Guestbook page. For Task 8, update both `<title>` and `<h1>` to `Guestbook – v2`.
- `Dockerfile` — builds an Nginx image, copies the HTML file, and exposes port 80.
- `deployment.yml` — Kubernetes Deployment and Service. Replace the image placeholder with your IBM Cloud Container Registry image.

## Build locally
```bash
docker build -t guestbook:v1 .
docker run --rm -p 8080:80 guestbook:v1
```
Open http://localhost:8080.

## Important
Use the exact IBM Cloud registry URL, namespace, cluster, and commands specified by your course. Do not commit API keys or tokens.

The assignment requires real terminal evidence from your environment. This ZIP does not include fabricated outputs for image pushes, HPA/autoscaling, deployment updates, rollout history, or rollback.
