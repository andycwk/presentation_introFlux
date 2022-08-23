kind create cluster 


flux bootstrap github \
  --owner=$GITHUB_USER \
  --repository=presentation_introFlux \
  --branch=main \
  --path=./clusters/local-dev \
  --personal

   watch flux get all -A
