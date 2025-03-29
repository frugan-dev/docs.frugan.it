```sh
cd docs/
rm -Rf build/
docker run --rm -it -v $(pwd):/docs sphinxdoc/sphinx bash
$# pip install sphinx_rtd_theme
$# make html
```