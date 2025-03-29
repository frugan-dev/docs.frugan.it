```sh
cd docs/
docker run --rm -it -v $(pwd):/docs sphinxdoc/sphinx bash
$# make html
```