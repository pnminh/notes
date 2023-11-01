## Red Hat Container APIs
### Swagger
https://catalog.redhat.com/api/containers/v1/ui/

### API
1. List all images
   ```
   $ curl https://catalog.redhat.com/api/containers/v1/repositories/registry/registry.access.redhat.com/repository/ubi8-minimal/images
   $ curl https://catalog.redhat.com/api/containers/v1/repositories/registry/registry.access.redhat.com/repository/ubi8-minimal/tag/latest
   $ curl https://catalog.redhat.com/api/containers/v1/repositories/registry/registry.access.redhat.com/repository/ubi8-minimal/tag/latest?page_size=1&page=1

   $ export RH_CATALOG_URL=https://catalog.redhat.com/api/containers
   $ curl $RH_CATALOG_URL/v1/tag-history/registry/registry.access.redhat.com/repository/ubi8/ubi-minimal/tag/latest

   ```
2. List tags for an image: 
   ```
   $ curl -sL https://registry.access.redhat.com/v2/ubi8-minimal/tags/list
   ```