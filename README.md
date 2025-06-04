# shim-assets

https://simple-x2acmlikgq-uw.a.run.app

https://console.cloud.google.com/run/detail/us-west1/simple?project=shim-assets

https://cloud.google.com/run/docs

```
docker build -t us-west1-docker.pkg.dev/shim-assets/cloud-run-source-deploy/simple samples/server/simple

docker push us-west1-docker.pkg.dev/shim-assets/cloud-run-source-deploy/simple

gcloud run deploy simple\
          --project=shim-assets\
          --platform=managed\
          --region=us-west1\
          --image=us-west1-docker.pkg.dev/shim-assets/cloud-run-source-deploy/simple\
          --allow-unauthenticated
