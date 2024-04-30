# Comparing `tmp/bo4e-202401.1.0rc2.tar.gz` & `tmp/bo4e-202401.1.1rc4.tar.gz`

## Comparing `bo4e-202401.1.0rc2.tar` & `bo4e-202401.1.1rc4.tar`

### file list

```diff
@@ -1,338 +1,346 @@
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/.pre-commit-config.yaml
--rw-r--r--   0        0        0    17211 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/.pylintrc
--rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/.readthedocs.yaml
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/CHANGELOG.rst
--rw-r--r--   0        0        0     5590 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/CONTRIBUTING.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/MANIFEST.in
--rw-r--r--   0        0        0     4683 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/README.rst
--rw-r--r--   0        0        0     3205 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/bo4e_schemas_create_release.py
--rw-r--r--   0        0        0     7964 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/generate_or_validate_json_schemas.py
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/requirements.in
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/requirements.txt
--rw-r--r--   0        0        0     3309 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tox.ini
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/.github/dependabot.yml
--rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/.github/ISSUE_TEMPLATE/funktionale-anforderung-an-den-bo4e-standard.md
--rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/.github/ISSUE_TEMPLATE/technisches-problem---python-specific-problem.md
--rw-r--r--   0        0        0     2497 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/.github/workflows/codeql-analysis.yml
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/.github/workflows/coverage.yml
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/.github/workflows/dependabot_automerge.yml
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/.github/workflows/formatting.yml
--rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/.github/workflows/linting.yml
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/.github/workflows/packaging_test.yml
--rw-r--r--   0        0        0     4385 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/.github/workflows/python-publish-scheduled.yml
--rw-r--r--   0        0        0     3806 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/.github/workflows/tests.yml
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/.vscode/settings.json
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/dev_requirements/requirements-coverage.in
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/dev_requirements/requirements-coverage.txt
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/dev_requirements/requirements-formatting.in
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/dev_requirements/requirements-formatting.txt
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/dev_requirements/requirements-json_schemas.in
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/dev_requirements/requirements-json_schemas.txt
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/dev_requirements/requirements-linting.in
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/dev_requirements/requirements-linting.txt
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/dev_requirements/requirements-packaging.in
--rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/dev_requirements/requirements-packaging.txt
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/dev_requirements/requirements-tests.in
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/dev_requirements/requirements-tests.txt
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/dev_requirements/requirements-type_check.in
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/dev_requirements/requirements-type_check.txt
--rw-r--r--   0        0        0     7602 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/docs/Makefile
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/docs/authors.rst
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/docs/changelog.rst
--rw-r--r--   0        0        0    11035 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/docs/conf.py
--rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/docs/index.rst
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/docs/license.rst
--rw-r--r--   0        0        0     2572 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/docs/release_workflow.rst
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/docs/requirements.in
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/docs/requirements.txt
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/docs/test_uml.py
--rw-r--r--   0        0        0    28433 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/docs/uml.py
--rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/docs/versioning.rst
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/docs/_static/bo4e-python-favicon.png
--rw-r--r--   0        0        0     4668 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/docs/_static/bo4e-python-favicon.svg
--rw-r--r--   0        0        0     4590 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/docs/_static/bo4e-python-logo.png
--rw-r--r--   0        0        0    26543 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/docs/_static/bo4e-python-logo.svg
--rw-r--r--   0        0        0   167661 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/docs/_static/bo4e-release-workflow.excalidraw
--rw-r--r--   0        0        0   512116 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/docs/_static/bo4e-release-workflow.png
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/_bo4e_python_version.py
--rw-r--r--   0        0        0    12614 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/__init__.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/py.typed
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/version.py
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/zusatzattribut.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/bo/__init__.py
--rw-r--r--   0        0        0     2576 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/bo/angebot.py
--rw-r--r--   0        0        0     3056 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/bo/ausschreibung.py
--rw-r--r--   0        0        0     2963 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/bo/buendelvertrag.py
--rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/bo/energiemenge.py
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/bo/fremdkosten.py
--rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/bo/geraet.py
--rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/bo/geschaeftsobjekt.py
--rw-r--r--   0        0        0     3493 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/bo/geschaeftspartner.py
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/bo/kosten.py
--rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/bo/lastgang.py
--rw-r--r--   0        0        0     5973 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/bo/marktlokation.py
--rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/bo/marktteilnehmer.py
--rw-r--r--   0        0        0     3353 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/bo/messlokation.py
--rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/bo/person.py
--rw-r--r--   0        0        0     2063 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/bo/preisblatt.py
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/bo/preisblattdienstleistung.py
--rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/bo/preisblatthardware.py
--rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/bo/preisblattkonzessionsabgabe.py
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/bo/preisblattmessung.py
--rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/bo/preisblattnetznutzung.py
--rw-r--r--   0        0        0     4822 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/bo/rechnung.py
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/bo/region.py
--rw-r--r--   0        0        0     2067 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/bo/regionaltarif.py
--rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/bo/standorteigenschaften.py
--rw-r--r--   0        0        0     2235 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/bo/tarif.py
--rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/bo/tarifinfo.py
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/bo/tarifkosten.py
--rw-r--r--   0        0        0     2023 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/bo/tarifpreisblatt.py
--rw-r--r--   0        0        0     3155 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/bo/vertrag.py
--rw-r--r--   0        0        0     2964 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/bo/zaehler.py
--rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/bo/zeitreihe.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/__init__.py
--rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/adresse.py
--rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/angebotsposition.py
--rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/angebotsteil.py
--rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/angebotsvariante.py
--rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/aufabschlag.py
--rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/aufabschlagproort.py
--rw-r--r--   0        0        0     3714 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/aufabschlagregional.py
--rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/aufabschlagstaffelproort.py
--rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/ausschreibungsdetail.py
--rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/ausschreibungslos.py
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/betrag.py
--rw-r--r--   0        0        0     2260 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/com.py
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/dienstleistung.py
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/energieherkunft.py
--rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/energiemix.py
--rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/fremdkostenblock.py
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/fremdkostenposition.py
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/geokoordinaten.py
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/katasteradresse.py
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/kontaktweg.py
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/konzessionsabgabe.py
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/kostenblock.py
--rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/kostenposition.py
--rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/kriteriumwert.py
--rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/marktgebietinfo.py
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/menge.py
--rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/messlokationszuordnung.py
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/positionsaufabschlag.py
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/preis.py
--rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/preisgarantie.py
--rw-r--r--   0        0        0     3227 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/preisposition.py
--rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/preisstaffel.py
--rw-r--r--   0        0        0     3045 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/rechnungsposition.py
--rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/regionalegueltigkeit.py
--rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/regionalepreisgarantie.py
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/regionalepreisstaffel.py
--rw-r--r--   0        0        0     3793 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/regionaleraufabschlag.py
--rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/regionaletarifpreisposition.py
--rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/regionskriterium.py
--rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/sigmoidparameter.py
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/standorteigenschaftengas.py
--rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/standorteigenschaftenstrom.py
--rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/steuerbetrag.py
--rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/tarifberechnungsparameter.py
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/tarifeinschraenkung.py
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/tarifpreis.py
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/tarifpreisposition.py
--rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/tarifpreispositionproort.py
--rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/tarifpreisstaffelproort.py
--rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/unterschrift.py
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/verbrauch.py
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/vertragskonditionen.py
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/vertragsteil.py
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/verwendungszweckpromarktrolle.py
--rw-r--r--   0        0        0     3110 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/zaehlwerk.py
--rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/zaehlzeitregister.py
--rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/zeitraum.py
--rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/zeitreihenwert.py
--rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/zeitspanne.py
--rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/zustaendigkeit.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/__init__.py
--rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/abgabeart.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/angebotsstatus.py
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/anrede.py
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/arithmetische_operation.py
--rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/artikelid.py
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/aufabschlagstyp.py
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/aufabschlagsziel.py
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/ausschreibungsportal.py
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/ausschreibungsstatus.py
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/ausschreibungstyp.py
--rw-r--r--   0        0        0     3598 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/bdewartikelnummer.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/befestigungsart.py
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/bemessungsgroesse.py
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/bilanzierungsmethode.py
--rw-r--r--   0        0        0     3853 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/dienstleistungstyp.py
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/energierichtung.py
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/erzeugungsart.py
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/gasqualitaet.py
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/gebiettyp.py
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/geraeteklasse.py
--rw-r--r--   0        0        0     3540 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/geraetetyp.py
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/geschaeftspartnerrolle.py
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/gueltigkeitstyp.py
--rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/kalkulationsmethode.py
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/kontaktart.py
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/kostenklasse.py
--rw-r--r--   0        0        0     2201 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/kundengruppe.py
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/kundengruppeka.py
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/kundentyp.py
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/landescode.py
--rw-r--r--   0        0        0     2641 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/leistungstyp.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/lokationstyp.py
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/marktrolle.py
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/medium.py
--rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/mengeneinheit.py
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/mengenoperator.py
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/messart.py
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/messgroesse.py
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/messpreistyp.py
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/messwerterfassung.py
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/messwertstatus.py
--rw-r--r--   0        0        0     4029 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/messwertstatuszusatz.py
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/netzebene.py
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/netznutzungrechnungsart.py
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/netznutzungrechnungstyp.py
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/oekolabel.py
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/oekozertifikat.py
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/organisationstyp.py
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/preisgarantietyp.py
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/preismodell.py
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/preisstatus.py
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/preistyp.py
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/rechnungslegung.py
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/rechnungsstatus.py
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/rechnungstyp.py
--rw-r--r--   0        0        0     2687 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/regionskriteriumtyp.py
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/registeranzahl.py
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/rollencodetyp.py
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/sparte.py
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/steuerkennzeichen.py
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/strenum.py
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/tarifkalkulationsmethode.py
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/tarifmerkmal.py
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/tarifregionskriterium.py
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/tariftyp.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/tarifzeit.py
--rw-r--r--   0        0        0     3997 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/themengebiet.py
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/titel.py
--rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/typ.py
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/verbrauchsart.py
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/vertragsart.py
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/vertragsform.py
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/vertragsstatus.py
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/verwendungszweck.py
--rw-r--r--   0        0        0     4475 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/voraussetzungen.py
--rw-r--r--   0        0        0     6464 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/waehrungscode.py
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/waehrungseinheit.py
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/waermenutzung.py
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/wertermittlungsverfahren.py
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/zaehlerauspraegung.py
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/zaehlergroesse.py
--rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/zaehlertyp.py
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/zaehlertypspezifikation.py
--rw-r--r--   0        0        0     3429 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/utils/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/__init__.py
--rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/serialization_helper.py
--rw-r--r--   0        0        0     3626 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_adresse.py
--rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_angebot.py
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_angebotsposition.py
--rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_angebotsteil.py
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_angebotsvariante.py
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_aufabschlag.py
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_aufabschlagproort.py
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_aufabschlagregional.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_aufabschlagstaffelproort.py
--rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_ausschreibung.py
--rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_ausschreibungsdetail.py
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_ausschreibungslos.py
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_betrag.py
--rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_buendelvertrag.py
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_energieherkunft.py
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_energiemenge.py
--rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_energiemix.py
--rw-r--r--   0        0        0     2094 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_enums.py
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_fremdkosten.py
--rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_fremdkostenblock.py
--rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_fremdkostenposition.py
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_geokoordinaten.py
--rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_geraet.py
--rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_geschaeftsobjekt.py
--rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_geschaeftspartner.py
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_import_enum.py
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_katasteradresse.py
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_kontakt.py
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_kosten.py
--rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_kostenblock.py
--rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_kostenposition.py
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_kriteriumswert.py
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_lastgang.py
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_marktgebietinfo.py
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_marktlokation.py
--rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_marktteilnehmer.py
--rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_menge.py
--rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_messlokation.py
--rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_messlokationszuordnung.py
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_person.py
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_positionsaufabschlag.py
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_preis.py
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_preisblatt.py
--rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_preisblatt_dienstleistung.py
--rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_preisblatt_hardware.py
--rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_preisblatt_konzessionsabgabe.py
--rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_preisblatt_messung.py
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_preisblattnetznutzung.py
--rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_preisgarantie.py
--rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_preisposition.py
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_preisstaffel.py
--rw-r--r--   0        0        0     6039 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_rechnung.py
--rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_rechnungsposition.py
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_region.py
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_regionalegueltigkeit.py
--rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_regionalepreisgarantie.py
--rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_regionalepreisstaffel.py
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_regionaleraufabschlag.py
--rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_regionaletarifpreisposition.py
--rw-r--r--   0        0        0     2162 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_regionaltarif.py
--rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_regionskriterium.py
--rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_sigmoidparameter.py
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_standorteigenschaften.py
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_standorteigenschaftengas.py
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_standorteigenschaftenstrom.py
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_steuerbetrag.py
--rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_tarif.py
--rw-r--r--   0        0        0     1489 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_tarifberechnungsparameter.py
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_tarifeinschraenkung.py
--rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_tarifinfo.py
--rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_tarifkosten.py
--rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_tarifpreis.py
--rw-r--r--   0        0        0     2091 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_tarifpreisblatt.py
--rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_tarifpreisposition.py
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_tarifpreispositionproort.py
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_tarifpreisstaffelproort.py
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_unterschrift.py
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_verbrauch.py
--rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_vertrag.py
--rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_vertragskonditionen.py
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_vertragsteil.py
--rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_zaehler.py
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_zeitraum.py
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_zeitreihe.py
--rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_zeitreihenwert.py
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_zeitspanne.py
--rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_zusatz_attribut.py
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/utils.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_data/test_data_adresse/test_data_adresse_missing_plz.json
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_data/test_data_adresse/test_data_adresse_only_required_fields.json
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_data/test_data_adresse/test_data_adresse_with_all_possible_fields.json
--rw-r--r--   0        0        0     2613 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/.gitignore
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/AUTHORS.rst
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/LICENSE.rst
--rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/pyproject.toml
--rw-r--r--   0        0        0     5936 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/PKG-INFO
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    17211 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/.pylintrc
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/CHANGELOG.rst
+-rw-r--r--   0        0        0     5590 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/CONTRIBUTING.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/MANIFEST.in
+-rw-r--r--   0        0        0     5748 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/README.rst
+-rw-r--r--   0        0        0     3205 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/bo4e_schemas_create_release.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/docker-compose.yml
+-rw-r--r--   0        0        0     8036 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/generate_or_validate_json_schemas.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/requirements.in
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/requirements.txt
+-rw-r--r--   0        0        0     3557 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tox.ini
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/.github/dependabot.yml
+-rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/.github/ISSUE_TEMPLATE/funktionale-anforderung-an-den-bo4e-standard.md
+-rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/.github/ISSUE_TEMPLATE/technisches-problem---python-specific-problem.md
+-rw-r--r--   0        0        0     2497 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/.github/workflows/coverage.yml
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/.github/workflows/dependabot_automerge.yml
+-rw-r--r--   0        0        0     2696 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/.github/workflows/docs_latest.yml
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/.github/workflows/formatting.yml
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/.github/workflows/linting.yml
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/.github/workflows/packaging_test.yml
+-rw-r--r--   0        0        0     4408 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/.github/workflows/python-publish-scheduled.yml
+-rw-r--r--   0        0        0     6475 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/.github/workflows/test_docs.yml
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/.vscode/settings.json
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/dev_requirements/requirements-coverage.in
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/dev_requirements/requirements-coverage.txt
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/dev_requirements/requirements-formatting.in
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/dev_requirements/requirements-formatting.txt
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/dev_requirements/requirements-json_schemas.in
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/dev_requirements/requirements-json_schemas.txt
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/dev_requirements/requirements-linting.in
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/dev_requirements/requirements-linting.txt
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/dev_requirements/requirements-packaging.in
+-rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/dev_requirements/requirements-packaging.txt
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/dev_requirements/requirements-tests.in
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/dev_requirements/requirements-tests.txt
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/dev_requirements/requirements-type_check.in
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/dev_requirements/requirements-type_check.txt
+-rw-r--r--   0        0        0     7602 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/docs/Makefile
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/docs/authors.rst
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/docs/changelog.rst
+-rw-r--r--   0        0        0    11523 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/docs/conf.py
+-rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/docs/index.rst
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/docs/license.rst
+-rw-r--r--   0        0        0     2572 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/docs/release_workflow.rst
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/docs/requirements.in
+-rw-r--r--   0        0        0     2422 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/docs/requirements.txt
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/docs/test_uml.py
+-rw-r--r--   0        0        0    28472 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/docs/uml.py
+-rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/docs/versioning.rst
+-rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/docs/_static/bo4e-python-favicon.png
+-rw-r--r--   0        0        0     4668 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/docs/_static/bo4e-python-favicon.svg
+-rw-r--r--   0        0        0     4590 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/docs/_static/bo4e-python-logo.png
+-rw-r--r--   0        0        0    26543 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/docs/_static/bo4e-python-logo.svg
+-rw-r--r--   0        0        0   167661 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/docs/_static/bo4e-release-workflow.excalidraw
+-rw-r--r--   0        0        0   512116 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/docs/_static/bo4e-release-workflow.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/docs/compatibility/__init__.py
+-rw-r--r--   0        0        0     9525 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/docs/compatibility/__main__.py
+-rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/docs/compatibility/change_schemas.py
+-rw-r--r--   0        0        0    13297 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/docs/compatibility/diff.py
+-rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/docs/compatibility/loader.py
+-rw-r--r--   0        0        0     2867 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/docs/compatibility/matrix.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/_bo4e_python_version.py
+-rw-r--r--   0        0        0    12614 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/__init__.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/py.typed
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/version.py
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/zusatzattribut.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/bo/__init__.py
+-rw-r--r--   0        0        0     2576 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/bo/angebot.py
+-rw-r--r--   0        0        0     3056 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/bo/ausschreibung.py
+-rw-r--r--   0        0        0     2963 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/bo/buendelvertrag.py
+-rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/bo/energiemenge.py
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/bo/fremdkosten.py
+-rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/bo/geraet.py
+-rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/bo/geschaeftsobjekt.py
+-rw-r--r--   0        0        0     3493 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/bo/geschaeftspartner.py
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/bo/kosten.py
+-rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/bo/lastgang.py
+-rw-r--r--   0        0        0     5973 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/bo/marktlokation.py
+-rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/bo/marktteilnehmer.py
+-rw-r--r--   0        0        0     3353 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/bo/messlokation.py
+-rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/bo/person.py
+-rw-r--r--   0        0        0     2063 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/bo/preisblatt.py
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/bo/preisblattdienstleistung.py
+-rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/bo/preisblatthardware.py
+-rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/bo/preisblattkonzessionsabgabe.py
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/bo/preisblattmessung.py
+-rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/bo/preisblattnetznutzung.py
+-rw-r--r--   0        0        0     4822 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/bo/rechnung.py
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/bo/region.py
+-rw-r--r--   0        0        0     2067 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/bo/regionaltarif.py
+-rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/bo/standorteigenschaften.py
+-rw-r--r--   0        0        0     2235 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/bo/tarif.py
+-rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/bo/tarifinfo.py
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/bo/tarifkosten.py
+-rw-r--r--   0        0        0     2023 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/bo/tarifpreisblatt.py
+-rw-r--r--   0        0        0     3155 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/bo/vertrag.py
+-rw-r--r--   0        0        0     2964 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/bo/zaehler.py
+-rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/bo/zeitreihe.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/__init__.py
+-rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/adresse.py
+-rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/angebotsposition.py
+-rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/angebotsteil.py
+-rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/angebotsvariante.py
+-rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/aufabschlag.py
+-rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/aufabschlagproort.py
+-rw-r--r--   0        0        0     3714 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/aufabschlagregional.py
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/aufabschlagstaffelproort.py
+-rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/ausschreibungsdetail.py
+-rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/ausschreibungslos.py
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/betrag.py
+-rw-r--r--   0        0        0     2260 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/com.py
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/dienstleistung.py
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/energieherkunft.py
+-rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/energiemix.py
+-rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/fremdkostenblock.py
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/fremdkostenposition.py
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/geokoordinaten.py
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/katasteradresse.py
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/kontaktweg.py
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/konzessionsabgabe.py
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/kostenblock.py
+-rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/kostenposition.py
+-rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/kriteriumwert.py
+-rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/marktgebietinfo.py
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/menge.py
+-rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/messlokationszuordnung.py
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/positionsaufabschlag.py
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/preis.py
+-rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/preisgarantie.py
+-rw-r--r--   0        0        0     3227 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/preisposition.py
+-rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/preisstaffel.py
+-rw-r--r--   0        0        0     3045 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/rechnungsposition.py
+-rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/regionalegueltigkeit.py
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/regionalepreisgarantie.py
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/regionalepreisstaffel.py
+-rw-r--r--   0        0        0     3793 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/regionaleraufabschlag.py
+-rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/regionaletarifpreisposition.py
+-rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/regionskriterium.py
+-rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/sigmoidparameter.py
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/standorteigenschaftengas.py
+-rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/standorteigenschaftenstrom.py
+-rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/steuerbetrag.py
+-rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/tarifberechnungsparameter.py
+-rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/tarifeinschraenkung.py
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/tarifpreis.py
+-rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/tarifpreisposition.py
+-rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/tarifpreispositionproort.py
+-rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/tarifpreisstaffelproort.py
+-rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/unterschrift.py
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/verbrauch.py
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/vertragskonditionen.py
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/vertragsteil.py
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/verwendungszweckpromarktrolle.py
+-rw-r--r--   0        0        0     3110 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/zaehlwerk.py
+-rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/zaehlzeitregister.py
+-rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/zeitraum.py
+-rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/zeitreihenwert.py
+-rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/zeitspanne.py
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/zustaendigkeit.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/__init__.py
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/abgabeart.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/angebotsstatus.py
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/anrede.py
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/arithmetische_operation.py
+-rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/artikelid.py
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/aufabschlagstyp.py
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/aufabschlagsziel.py
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/ausschreibungsportal.py
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/ausschreibungsstatus.py
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/ausschreibungstyp.py
+-rw-r--r--   0        0        0     3598 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/bdewartikelnummer.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/befestigungsart.py
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/bemessungsgroesse.py
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/bilanzierungsmethode.py
+-rw-r--r--   0        0        0     3853 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/dienstleistungstyp.py
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/energierichtung.py
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/erzeugungsart.py
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/gasqualitaet.py
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/gebiettyp.py
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/geraeteklasse.py
+-rw-r--r--   0        0        0     3540 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/geraetetyp.py
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/geschaeftspartnerrolle.py
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/gueltigkeitstyp.py
+-rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/kalkulationsmethode.py
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/kontaktart.py
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/kostenklasse.py
+-rw-r--r--   0        0        0     2201 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/kundengruppe.py
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/kundengruppeka.py
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/kundentyp.py
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/landescode.py
+-rw-r--r--   0        0        0     2641 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/leistungstyp.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/lokationstyp.py
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/marktrolle.py
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/medium.py
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/mengeneinheit.py
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/mengenoperator.py
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/messart.py
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/messgroesse.py
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/messpreistyp.py
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/messwerterfassung.py
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/messwertstatus.py
+-rw-r--r--   0        0        0     4029 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/messwertstatuszusatz.py
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/netzebene.py
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/netznutzungrechnungsart.py
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/netznutzungrechnungstyp.py
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/oekolabel.py
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/oekozertifikat.py
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/organisationstyp.py
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/preisgarantietyp.py
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/preismodell.py
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/preisstatus.py
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/preistyp.py
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/rechnungslegung.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/rechnungsstatus.py
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/rechnungstyp.py
+-rw-r--r--   0        0        0     2687 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/regionskriteriumtyp.py
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/registeranzahl.py
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/rollencodetyp.py
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/sparte.py
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/steuerkennzeichen.py
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/strenum.py
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/tarifkalkulationsmethode.py
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/tarifmerkmal.py
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/tarifregionskriterium.py
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/tariftyp.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/tarifzeit.py
+-rw-r--r--   0        0        0     3997 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/themengebiet.py
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/titel.py
+-rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/typ.py
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/verbrauchsart.py
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/vertragsart.py
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/vertragsform.py
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/vertragsstatus.py
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/verwendungszweck.py
+-rw-r--r--   0        0        0     4475 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/voraussetzungen.py
+-rw-r--r--   0        0        0     6464 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/waehrungscode.py
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/waehrungseinheit.py
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/waermenutzung.py
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/wertermittlungsverfahren.py
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/zaehlerauspraegung.py
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/zaehlergroesse.py
+-rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/zaehlertyp.py
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/zaehlertypspezifikation.py
+-rw-r--r--   0        0        0     3429 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/utils/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/__init__.py
+-rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/serialization_helper.py
+-rw-r--r--   0        0        0     3626 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_adresse.py
+-rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_angebot.py
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_angebotsposition.py
+-rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_angebotsteil.py
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_angebotsvariante.py
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_aufabschlag.py
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_aufabschlagproort.py
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_aufabschlagregional.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_aufabschlagstaffelproort.py
+-rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_ausschreibung.py
+-rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_ausschreibungsdetail.py
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_ausschreibungslos.py
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_betrag.py
+-rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_buendelvertrag.py
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_energieherkunft.py
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_energiemenge.py
+-rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_energiemix.py
+-rw-r--r--   0        0        0     2094 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_enums.py
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_fremdkosten.py
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_fremdkostenblock.py
+-rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_fremdkostenposition.py
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_geokoordinaten.py
+-rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_geraet.py
+-rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_geschaeftsobjekt.py
+-rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_geschaeftspartner.py
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_import_enum.py
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_katasteradresse.py
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_kontakt.py
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_kosten.py
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_kostenblock.py
+-rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_kostenposition.py
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_kriteriumswert.py
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_lastgang.py
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_marktgebietinfo.py
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_marktlokation.py
+-rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_marktteilnehmer.py
+-rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_menge.py
+-rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_messlokation.py
+-rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_messlokationszuordnung.py
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_person.py
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_positionsaufabschlag.py
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_preis.py
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_preisblatt.py
+-rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_preisblatt_dienstleistung.py
+-rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_preisblatt_hardware.py
+-rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_preisblatt_konzessionsabgabe.py
+-rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_preisblatt_messung.py
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_preisblattnetznutzung.py
+-rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_preisgarantie.py
+-rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_preisposition.py
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_preisstaffel.py
+-rw-r--r--   0        0        0     6039 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_rechnung.py
+-rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_rechnungsposition.py
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_region.py
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_regionalegueltigkeit.py
+-rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_regionalepreisgarantie.py
+-rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_regionalepreisstaffel.py
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_regionaleraufabschlag.py
+-rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_regionaletarifpreisposition.py
+-rw-r--r--   0        0        0     2162 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_regionaltarif.py
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_regionskriterium.py
+-rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_sigmoidparameter.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_standorteigenschaften.py
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_standorteigenschaftengas.py
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_standorteigenschaftenstrom.py
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_steuerbetrag.py
+-rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_tarif.py
+-rw-r--r--   0        0        0     1489 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_tarifberechnungsparameter.py
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_tarifeinschraenkung.py
+-rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_tarifinfo.py
+-rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_tarifkosten.py
+-rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_tarifpreis.py
+-rw-r--r--   0        0        0     2091 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_tarifpreisblatt.py
+-rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_tarifpreisposition.py
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_tarifpreispositionproort.py
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_tarifpreisstaffelproort.py
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_unterschrift.py
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_verbrauch.py
+-rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_vertrag.py
+-rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_vertragskonditionen.py
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_vertragsteil.py
+-rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_zaehler.py
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_zeitraum.py
+-rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_zeitreihe.py
+-rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_zeitreihenwert.py
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_zeitspanne.py
+-rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_zusatz_attribut.py
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/utils.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_data/test_data_adresse/test_data_adresse_missing_plz.json
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_data/test_data_adresse/test_data_adresse_only_required_fields.json
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_data/test_data_adresse/test_data_adresse_with_all_possible_fields.json
+-rw-r--r--   0        0        0     2649 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/.gitignore
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/AUTHORS.rst
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/LICENSE.rst
+-rw-r--r--   0        0        0     2584 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/pyproject.toml
+-rw-r--r--   0        0        0     7050 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/PKG-INFO
```

### Comparing `bo4e-202401.1.0rc2/.pre-commit-config.yaml` & `bo4e-202401.1.1rc4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/.pylintrc` & `bo4e-202401.1.1rc4/.pylintrc`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/CONTRIBUTING.md` & `bo4e-202401.1.1rc4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/README.rst` & `bo4e-202401.1.1rc4/README.rst`

 * *Files 25% similar despite different names*

```diff
@@ -48,15 +48,30 @@
 * Generell sollen Verweise zwischen zwei BOs bi-direktional sein, zwischen BOs und COMs aber nur unidirektional (z.B. soll jeder Zähler wissen zu welcher Messlokation er gehört aber eine Adresse muss nicht wissen, welchem Geschäftspartner, welcher Messlokation oder welcher Rechnung sie zugeordnet ist).
 * COMs können zwar weitere COMs beinhalten, jedoch sollte dies nicht dafür genutzt werden von einem COM eines BOs auf das COM eines anderen BOs zu verweisen.
   Bsp.: Die Adresse in Ansprechpartner ist identisch zur Lokationsadresse in der Marktlokation. Dann sollen beide Adressen als vollständiges COM dargestellt werden, statt nur als Verweis von einer Adresse auf die andere.
 * Oder anders formuliert: wir können aus einem BO oder einem COM auf ein anderes BO verweisen.
 
 Dokumentation / Fragen und Anregungen zum BO4E Datenmodell
 ==========================================================
-Eine Dokumentation des Datenmodells und JSON Schemata zur Erzeugung von Beispieldaten finden sich auf `read the docs <https://bo4e-python.readthedocs.io/en/latest/api/modules.html>`_.
+Die Dokumentation ist verfügbar unter `<https://bo4e.github.io/BO4E-python/>`_.
+Die Doku wird erst seit Version `v202401.0.3 <https://bo4e.github.io/BO4E-python/v202401.0.3>`_ mittels
+GitHub Pages gehosted.
+Die früheren Versionen sind auf `read the docs <https://bo4e-python.readthedocs.io/en/latest/api/modules.html>`_
+einsehbar.
+
+Unter `/latest` findet sich die Dokumentation des aktuellen Stands des main-Branches. `/stable` zeigt immer auf die
+letzte veröffentlichte Version (Release candidates ausgeschlossen).
+Zusätzlich ist jede Version (inklusive Release candidates) unter `/v<version>` auffindbar.
+
+Die Doku bietet eine Übersicht über alle Klassen und Attribute, die im BO4E Standard definiert sind. Außerdem
+werden alle Beziehungen zwischen den Klassen durch Diagramme visualisiert. Die JSON-Schemas sind ebenfalls verlinkt.
+Alternativ können die JSON-Schemas auch direkt von GitHub heruntergeladen werden: `<https://github.com/bo4e/BO4E-Schemas>`_.
+Seit Version `v202401.1.1 <https://bo4e.github.io/BO4E-python/v202401.1.1>`_ gibt es zusätzlich eine
+`Kompatibilitätsmatrix <https://bo4e.github.io/BO4E-python/v202401.1.1/changelog.html>`_,
+die für jedes Objekt zeigt, zwischen welchen Versionen es einen "breaking change" gab.
 
 Bei Fragen oder Anregungen, bitte `einfach ein Issue in diesem Repo aufmachen <https://github.com/Hochfrequenz/BO4E-python/issues/new?assignees=&labels=BO4E+Enhancement+Proposal&template=funktionale-anforderung-an-den-bo4e-standard.md&title=Ein+aussagekr%C3%A4ftiger+Titel%3A+Hunde-+und+Katzentarife+k%C3%B6nnen+nicht+abgebildet+werden>`_.
 
 Code Beiträge
 =============
 Änderungsvorschläge (sowohl an das Datenmodell als auch an die Implementierung in Python) können direkt als Code in Form von Pull Requests eingereicht werden.
 Details dazu finden sich im `Contribution Guide`_.
```

### Comparing `bo4e-202401.1.0rc2/bo4e_schemas_create_release.py` & `bo4e-202401.1.1rc4/bo4e_schemas_create_release.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/generate_or_validate_json_schemas.py` & `bo4e-202401.1.1rc4/generate_or_validate_json_schemas.py`

 * *Files 1% similar despite different names*

```diff
@@ -187,14 +187,15 @@
     required=False,
     type=click.STRING,
     envvar="TARGET_VERSION",
     default="v0.0.0",
 )
 def generate_or_validate_json_schemas(mode: Literal["validate", "generate"], target_version: str) -> None:
     """generate json schemas for all BOs and COMs"""
+    _logger.debug("Mode: %s, target version: %s", mode, target_version)
     packages = ["bo", "com", "enum"]
 
     if mode == "generate":
         delete_json_schemas(packages)
 
     namespace = get_namespace(packages)
     namespace[ZusatzAttribut.__name__] = ("", "zusatzattribut", ZusatzAttribut)
```

### Comparing `bo4e-202401.1.0rc2/tox.ini` & `bo4e-202401.1.1rc4/tox.ini`

 * *Files 4% similar despite different names*

```diff
@@ -24,28 +24,30 @@
     -r requirements.txt
     -r dev_requirements/requirements-linting.txt
     {[testenv:docs]deps}
     {[testenv:generate_json_schemas]deps}
 commands =
     pylint src/bo4e
     pylint docs/uml.py
+    pylint docs/compatibility
     pylint generate_or_validate_json_schemas.py
 
 [testenv:type_check]
 usedevelop = True
 # the type_check environment checks the type hints using mypy
 deps =
     -rrequirements.txt
     {[testenv:docs]deps}
     {[testenv:generate_json_schemas]deps}
     -r dev_requirements/requirements-type_check.txt
 commands =
     mypy --show-error-codes src/bo4e
     mypy --show-error-codes tests
     mypy --show-error-codes docs/uml.py
+    mypy --show-error-codes docs/compatibility
     mypy --show-error-codes generate_or_validate_json_schemas.py
     # add single files (ending with .py) or packages here
 
 [testenv:coverage]
 usedevelop = True
 deps =
     {[testenv:tests]deps}
@@ -76,18 +78,23 @@
     pre-commit install
 
 
 [testenv:docs]
 deps =
     -r requirements.txt
     -r docs/requirements.txt
+    {[testenv:generate_json_schemas]deps}
 # any dependency added here should also be added in docs/requirements.in and docs/requirements.txt respectively
+setenv =
+    TARGET_VERSION = {env:TARGET_VERSION:local}
+    SPHINX_DOCS_RELEASE = {env:TARGET_VERSION:local}
+    SPHINX_DOCS_VERSION = {env:TARGET_VERSION:local}
 commands =
-    sphinx-build -W -b html -d {envtmpdir}/doctrees docs {envtmpdir}/html
-    sphinx-build -n -T -W -b doctest -d {envtmpdir}/doctrees docs docs/_build/html
+    {[testenv:generate_json_schemas]commands}
+    sphinx-build -T -W -b html -d {envtmpdir}/doctrees docs {envtmpdir}/html
     python -m doctest README.rst
 
 
 [testenv:bo4e-from-pip]
 basepython = python3.10
 skip_install = true
 deps = -r dev_requirements/requirements-tests.txt
```

### Comparing `bo4e-202401.1.0rc2/.github/dependabot.yml` & `bo4e-202401.1.1rc4/.github/dependabot.yml`

 * *Files 8% similar despite different names*

```diff
@@ -15,7 +15,9 @@
     schedule:
       interval: "weekly"
   # Maintain dependencies for GitHub Actions
   - package-ecosystem: "github-actions"
     directory: "/"
     schedule:
       interval: "daily"
+    ignore:
+      - dependency-name: "sphinx-notes/pages"
```

### Comparing `bo4e-202401.1.0rc2/.github/ISSUE_TEMPLATE/funktionale-anforderung-an-den-bo4e-standard.md` & `bo4e-202401.1.1rc4/.github/ISSUE_TEMPLATE/funktionale-anforderung-an-den-bo4e-standard.md`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/.github/ISSUE_TEMPLATE/technisches-problem---python-specific-problem.md` & `bo4e-202401.1.1rc4/.github/ISSUE_TEMPLATE/technisches-problem---python-specific-problem.md`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/.github/workflows/codeql-analysis.yml` & `bo4e-202401.1.1rc4/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/.github/workflows/coverage.yml` & `bo4e-202401.1.1rc4/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/.github/workflows/dependabot_automerge.yml` & `bo4e-202401.1.1rc4/.github/workflows/dependabot_automerge.yml`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/.github/workflows/linting.yml` & `bo4e-202401.1.1rc4/.github/workflows/linting.yml`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/.github/workflows/packaging_test.yml` & `bo4e-202401.1.1rc4/.github/workflows/packaging_test.yml`

 * *Files 25% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 on: [pull_request]
 jobs:
   check_packaging:
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
-        python-version: ["3.11"]
+        python-version: ["3.9", "3.10", "3.11", "3.12"]
         os: [ubuntu-latest]
     steps:
       - uses: actions/checkout@v4
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
```

### Comparing `bo4e-202401.1.0rc2/.github/workflows/python-publish-scheduled.yml` & `bo4e-202401.1.1rc4/.github/workflows/python-publish-scheduled.yml`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     - cron: '23 1 1 1,7 *'
 
 jobs:
   tests:
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
-        python-version: ["3.11"]
+        python-version: ["3.9", "3.10", "3.11", "3.12"]
         os: [ubuntu-latest]
     steps:
       - uses: actions/checkout@v4
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
```

### Comparing `bo4e-202401.1.0rc2/.github/workflows/tests.yml` & `bo4e-202401.1.1rc4/.github/workflows/tests.yml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 on: [push,pull_request]
 jobs:
   tests:
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
-        python-version: ["3.10", "3.11", "3.12"]
+        python-version: ["3.9", "3.10", "3.11", "3.12"]
         os: [ubuntu-latest]
     steps:
       - uses: actions/checkout@v4
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
```

### Comparing `bo4e-202401.1.0rc2/dev_requirements/requirements-packaging.txt` & `bo4e-202401.1.1rc4/dev_requirements/requirements-packaging.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,41 +1,38 @@
+# SHA1:93e4fbf2b6cce1574fe3d5315360512fa9927699
 #
-# This file is autogenerated by pip-compile with Python 3.12
-# by the following command:
+# This file is autogenerated by pip-compile-multi
+# To update, run:
 #
-#    pip-compile '.\dev_requirements\requirements-packaging.in'
+#    pip-compile-multi
 #
+backports-tarfile==1.1.1
+    # via jaraco-context
 build==1.2.1
-    # via -r requirements-packaging.in
+    # via -r dev_requirements\requirements-packaging.in
 certifi==2024.2.2
     # via requests
-cffi==1.16.0
-    # via cryptography
 charset-normalizer==3.3.2
     # via requests
-cryptography==42.0.5
-    # via secretstorage
-docutils==0.20.1
+colorama==0.4.6
+    # via build
+docutils==0.21.1
     # via readme-renderer
 idna==3.7
     # via requests
 importlib-metadata==7.1.0
     # via
     #   keyring
     #   twine
 jaraco-classes==3.4.0
     # via keyring
-jaraco-context==5.0.0
+jaraco-context==5.3.0
     # via keyring
-jaraco-functools==4.0.0
+jaraco-functools==4.0.1
     # via keyring
-jeepney==0.8.0
-    # via
-    #   keyring
-    #   secretstorage
 keyring==25.1.0
     # via twine
 markdown-it-py==3.0.0
     # via rich
 mdurl==0.1.2
     # via markdown-it-py
 more-itertools==10.2.0
@@ -44,37 +41,35 @@
     #   jaraco-functools
 nh3==0.2.17
     # via readme-renderer
 packaging==24.0
     # via build
 pkginfo==1.10.0
     # via twine
-pycparser==2.22
-    # via cffi
 pygments==2.17.2
     # via
     #   readme-renderer
     #   rich
 pyproject-hooks==1.0.0
     # via build
+pywin32-ctypes==0.2.2
+    # via keyring
 readme-renderer==43.0
     # via twine
 requests==2.31.0
     # via
     #   requests-toolbelt
     #   twine
 requests-toolbelt==1.0.0
     # via twine
 rfc3986==2.0.0
     # via twine
 rich==13.7.1
     # via twine
-secretstorage==3.3.3
-    # via keyring
 twine==5.0.0
-    # via -r requirements-packaging.in
+    # via -r dev_requirements\requirements-packaging.in
 urllib3==2.2.1
     # via
     #   requests
     #   twine
 zipp==3.18.1
     # via importlib-metadata
```

### Comparing `bo4e-202401.1.0rc2/dev_requirements/requirements-type_check.txt` & `bo4e-202401.1.1rc4/dev_requirements/requirements-type_check.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,29 @@
+# SHA1:9a286c239b1bb587f83dac5fba3e8a2ebfa4029b
 #
-# This file is autogenerated by pip-compile with Python 3.11
-# by the following command:
+# This file is autogenerated by pip-compile-multi
+# To update, run:
 #
-#    pip-compile '.\requirements-type_check.in'
+#    pip-compile-multi
 #
 iniconfig==2.0.0
     # via pytest
-mypy==1.9.0
+mypy==1.10.0
     # via -r requirements-type_check.in
 mypy-extensions==1.0.0
     # via mypy
-networkx==3.2
+networkx==3.3
     # via networkx-stubs
 networkx-stubs==0.0.1
     # via -r requirements-type_check.in
-packaging==23.1
+packaging==24.0
     # via pytest
-pluggy==1.4.0
+pluggy==1.5.0
     # via pytest
-pytest==8.1.1
+pytest==8.2.0
     # via -r requirements-type_check.in
 types-requests==2.31.0.20240406
     # via -r requirements-type_check.in
-typing-extensions==4.8.0
+typing-extensions==4.11.0
     # via mypy
-urllib3==2.0.7
+urllib3==2.2.1
     # via types-requests
```

### Comparing `bo4e-202401.1.0rc2/docs/Makefile` & `bo4e-202401.1.1rc4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/docs/conf.py` & `bo4e-202401.1.1rc4/docs/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,30 +3,31 @@
 # This file is execfile()d with the current directory set to its containing dir.
 #
 # Note that not all possible configuration values are present in this
 # autogenerated file.
 #
 # All configuration values have a default; values that are commented out
 # serve to show the default.
-
 import inspect
 import os
 import shutil
 import sys
 
 __location__ = os.path.join(os.getcwd(), os.path.dirname(inspect.getfile(inspect.currentframe())))
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 from pathlib import Path
 
 sys.path.insert(0, os.path.join(__location__, "../src"))
 sys.path.insert(0, os.path.join(__location__, "../docs"))
+sys.path.insert(0, os.path.join(__location__, "../docs/compatibility"))
 import uml
+from compatibility.__main__ import create_tables_for_doc
 
 # import package bo4e to clarify namespaces and prevent circular import errors
 from bo4e import *
 
 # -- Run sphinx-apidoc ------------------------------------------------------
 # This hack is necessary since RTD does not issue `sphinx-apidoc` before running
 # `sphinx-build -b html . _build/html`. See Issue:
@@ -93,23 +94,14 @@
 # The master toctree document.
 master_doc = "index"
 
 # General information about the project.
 project = "bo4e"
 copyright = "2022, Hochfrequenz GmbH"
 
-# The version info for the project you're documenting, acts as replacement for
-# |version| and |release|, also used in various other places throughout the
-# built documents.
-#
-# The short X.Y version.
-version = ""  # Is set by calling `setup.py docs`
-# The full version, including alpha/beta/rc tags.
-release = ""  # Is set by calling `setup.py docs`
-
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 # language = None
 
 # There are two options for replacing |today|: either, you set today to some
 # non-false value, then it is used:
 # today = ''
@@ -172,16 +164,24 @@
 }
 
 # Add any paths that contain custom themes here, relative to this directory.
 # html_theme_path = []
 
 # The name for this set of Sphinx documents.  If None, it defaults to
 # "<project> v<release> documentation".
-from bo4e import __gh_version__ as release
-from bo4e import __version__ as version
+# Note: For the deployment to GitHub Pages the release and version values will
+# be set by the action. This is to support things like /latest or /stable.
+if "release" not in globals():
+    release = os.getenv("SPHINX_DOCS_RELEASE")
+    if release is None:
+        from bo4e import __gh_version__ as release
+if "version" not in globals():
+    version = os.getenv("SPHINX_DOCS_VERSION")
+    if version is None:
+        from bo4e import __version__ as version
 
 print(f"Got version = {version} from __version__")
 print(f"Got release = {release} from __gh_version__")
 
 # A shorter title for the navigation bar.  Default is the same as html_title.
 # html_short_title = None
 
@@ -305,16 +305,22 @@
 intersphinx_mapping = {
     "sphinx": ("http://www.sphinx-doc.org/en/stable", None),
     "python": ("https://docs.python.org/" + python_version, None),
 }
 
 # Create UML diagrams in plantuml format. Compile these into svg files into the _static folder.
 # See docs/uml.py for more details.
-uml.LINK_URI_BASE = f"https://bo4e-python.readthedocs.io/en/{release}"
+if release != "local":
+    uml.LINK_URI_BASE = f"https://bo4e.github.io/BO4E-python/{release}"
 _exec_plantuml = Path(__location__) / "plantuml.jar"
 _network, _namespaces_to_parse = uml.build_network(Path(module_dir), uml.PlantUMLNetwork)
 print(_network)
 uml.write_class_umls(_network, _namespaces_to_parse, Path(output_dir) / "uml")
 print("Created uml files.")
 
-uml.compile_files_kroki(Path(output_dir) / "uml", Path(output_dir).parent / "_static" / "images")
+uml.compile_files_kroki(Path(output_dir) / "uml", Path(output_dir).parent / "_static" / "images", locally_hosted=True)
 print(f"Compiled uml files into svg using kroki.")
+
+# Create compatibility matrix
+compatibility_matrix_output_file = Path(__file__).parent / "compatibility_matrix.csv"
+gh_token = os.getenv("GITHUB_ACCESS_TOKEN") or os.getenv("GITHUB_TOKEN")
+create_tables_for_doc(compatibility_matrix_output_file, release, last_n_versions=0, gh_token=gh_token)
```

### Comparing `bo4e-202401.1.0rc2/docs/index.rst` & `bo4e-202401.1.1rc4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/docs/release_workflow.rst` & `bo4e-202401.1.1rc4/docs/release_workflow.rst`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/docs/requirements.txt` & `bo4e-202401.1.1rc4/docs/requirements.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,67 +1,97 @@
 #
-# This file is autogenerated by pip-compile with Python 3.11
+# This file is autogenerated by pip-compile with Python 3.12
 # by the following command:
 #
 #    pip-compile '.\docs\requirements.in'
 #
 alabaster==0.7.13
     # via sphinx
 annotated-types==0.5.0
     # via pydantic
 babel==2.12.1
     # via sphinx
+bo4e-schema-tool==0.0.7
+    # via -r .\docs\requirements.in
 certifi==2023.7.22
     # via requests
+cffi==1.16.0
+    # via
+    #   cryptography
+    #   pynacl
 charset-normalizer==2.1.0
     # via requests
+click==8.1.7
+    # via bo4e-schema-tool
+colorama==0.4.6
+    # via
+    #   click
+    #   sphinx
+cryptography==42.0.5
+    # via pyjwt
+deprecated==1.2.14
+    # via pygithub
 docutils==0.18.1
     # via
     #   sphinx
     #   sphinx-rtd-theme
 idna==3.7
     # via requests
 imagesize==1.4.1
     # via sphinx
 iso3166==2.1.1
-    # via -r requirements.in
+    # via -r .\docs\requirements.in
 jinja2==3.1.3
     # via sphinx
 markupsafe==2.1.3
     # via jinja2
-networkx==3.2
-    # via -r requirements.in
-packaging==23.1
+more-itertools==10.2.0
+    # via bo4e-schema-tool
+networkx==3.3
+    # via -r .\docs\requirements.in
+packaging==24.0
     # via sphinx
+pycparser==2.21
+    # via cffi
 pydantic==2.4.2
-    # via -r requirements.in
+    # via
+    #   -r .\docs\requirements.in
+    #   bo4e-schema-tool
 pydantic-core==2.10.1
     # via pydantic
+pygithub==2.2.0
+    # via bo4e-schema-tool
 pygments==2.16.1
     # via sphinx
 pyhumps==3.8.0
-    # via -r requirements.in
+    # via -r .\docs\requirements.in
+pyjwt[crypto]==2.8.0
+    # via pygithub
+pynacl==1.5.0
+    # via pygithub
 requests==2.31.0
     # via
-    #   -r requirements.in
+    #   -r .\docs\requirements.in
+    #   bo4e-schema-tool
+    #   pygithub
     #   sphinx
 snowballstemmer==2.2.0
     # via sphinx
 sphinx==7.2.6
     # via
-    #   -r requirements.in
+    #   -r .\docs\requirements.in
     #   sphinx-rtd-theme
     #   sphinxcontrib-applehelp
     #   sphinxcontrib-devhelp
     #   sphinxcontrib-htmlhelp
     #   sphinxcontrib-jquery
     #   sphinxcontrib-qthelp
     #   sphinxcontrib-serializinghtml
 sphinx-rtd-theme==1.3.0
-    # via -r requirements.in
+    # via -r .\docs\requirements.in
 sphinxcontrib-applehelp==1.0.7
     # via sphinx
 sphinxcontrib-devhelp==1.0.5
     # via sphinx
 sphinxcontrib-htmlhelp==2.0.4
     # via sphinx
 sphinxcontrib-jquery==4.1
@@ -69,15 +99,19 @@
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
 sphinxcontrib-qthelp==1.0.6
     # via sphinx
 sphinxcontrib-serializinghtml==1.1.9
     # via sphinx
 typeguard==4.1.5
-    # via -r requirements.in
-typing-extensions==4.8.0
+    # via -r .\docs\requirements.in
+typing-extensions==4.11.0
     # via
     #   pydantic
     #   pydantic-core
-    #   typeguard
-urllib3==2.0.7
-    # via requests
+    #   pygithub
+urllib3==2.2.1
+    # via
+    #   pygithub
+    #   requests
+wrapt==1.16.0
+    # via deprecated
```

### Comparing `bo4e-202401.1.0rc2/docs/uml.py` & `bo4e-202401.1.1rc4/docs/uml.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,19 +75,16 @@
 being inherited by all classes in this project. Therefore, their namespace starts with the respective class e.g.
 `bo4e.bo.angebot.Angebot.ConstrainedStr`.
 """
 
 #: Define shorthand for Cardinality type since none of the values have to be provided.
 Cardinality = tuple[str, str]
 
-#: Define the link base URI used in svg links
-LINK_URI_BASE = "https://bo4e-python.readthedocs.io/en/latest"
-
-# link domain to test links only local.
-# LINK_URI_BASE = f"file:///{Path.cwd().parent}/.tox/docs/tmp/html"
+#: Define the link base URI used in svg links. Will be overridden by conf.py.
+LINK_URI_BASE = f"file:///{Path(__file__).parents[1]}/.tox/docs/tmp/html"
 
 
 class _UMLNetworkABC(nx.MultiDiGraph, metaclass=ABCMeta):
     """
     Defines the abstract base class for all UML-Parsers. Currently, there is only a Plantuml-parser, but you can easily
     add a parser by implementing all abstract methods in a subclass.
     """
@@ -564,20 +561,23 @@
                 through_field=model_field,
                 card1=None,
                 card2=field_card,
             )
     # ------------------------------------------------------------------------------------------------------------------
 
 
-def compile_files_kroki(input_dir: Path, output_dir: Path) -> None:
+def compile_files_kroki(input_dir: Path, output_dir: Path, locally_hosted: bool = False) -> None:
     """
     Compiles all plantuml files inside `input_dir` (recursive) to svg's in `output_dir` with the same subpath as in
     `input_dir`. Files are compiled using web service of [kroki](https://kroki.io)
     """
-    url = "https://kroki.io"
+    if locally_hosted:
+        url = "http://localhost:8000"
+    else:
+        url = "https://kroki.io"
     for root, _, files in os.walk(input_dir):
         for file in files:
             with open(os.path.join(root, file), "r", encoding="utf-8") as uml_file:
                 answer = requests.post(
                     url,
                     json={"diagram_source": uml_file.read(), "diagram_type": "plantuml", "output_format": "svg"},
                     timeout=15,
```

### Comparing `bo4e-202401.1.0rc2/docs/versioning.rst` & `bo4e-202401.1.1rc4/docs/versioning.rst`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/docs/_static/bo4e-python-favicon.png` & `bo4e-202401.1.1rc4/docs/_static/bo4e-python-favicon.png`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/docs/_static/bo4e-python-favicon.svg` & `bo4e-202401.1.1rc4/docs/_static/bo4e-python-favicon.svg`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/docs/_static/bo4e-python-logo.png` & `bo4e-202401.1.1rc4/docs/_static/bo4e-python-logo.png`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/docs/_static/bo4e-python-logo.svg` & `bo4e-202401.1.1rc4/docs/_static/bo4e-python-logo.svg`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/docs/_static/bo4e-release-workflow.excalidraw` & `bo4e-202401.1.1rc4/docs/_static/bo4e-release-workflow.excalidraw`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/docs/_static/bo4e-release-workflow.png` & `bo4e-202401.1.1rc4/docs/_static/bo4e-release-workflow.png`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/__init__.py` & `bo4e-202401.1.1rc4/src/bo4e/__init__.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/version.py` & `bo4e-202401.1.1rc4/src/bo4e/version.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/zusatzattribut.py` & `bo4e-202401.1.1rc4/src/bo4e/zusatzattribut.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/bo/angebot.py` & `bo4e-202401.1.1rc4/src/bo4e/bo/angebot.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/bo/ausschreibung.py` & `bo4e-202401.1.1rc4/src/bo4e/bo/ausschreibung.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/bo/buendelvertrag.py` & `bo4e-202401.1.1rc4/src/bo4e/bo/buendelvertrag.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/bo/energiemenge.py` & `bo4e-202401.1.1rc4/src/bo4e/bo/energiemenge.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/bo/fremdkosten.py` & `bo4e-202401.1.1rc4/src/bo4e/bo/fremdkosten.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/bo/geraet.py` & `bo4e-202401.1.1rc4/src/bo4e/bo/geraet.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/bo/geschaeftsobjekt.py` & `bo4e-202401.1.1rc4/src/bo4e/bo/geschaeftsobjekt.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/bo/geschaeftspartner.py` & `bo4e-202401.1.1rc4/src/bo4e/bo/geschaeftspartner.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/bo/kosten.py` & `bo4e-202401.1.1rc4/src/bo4e/bo/kosten.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/bo/lastgang.py` & `bo4e-202401.1.1rc4/src/bo4e/bo/lastgang.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/bo/marktlokation.py` & `bo4e-202401.1.1rc4/src/bo4e/bo/marktlokation.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/bo/marktteilnehmer.py` & `bo4e-202401.1.1rc4/src/bo4e/bo/marktteilnehmer.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/bo/messlokation.py` & `bo4e-202401.1.1rc4/src/bo4e/bo/messlokation.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/bo/person.py` & `bo4e-202401.1.1rc4/src/bo4e/bo/person.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/bo/preisblatt.py` & `bo4e-202401.1.1rc4/src/bo4e/bo/preisblatt.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/bo/preisblattdienstleistung.py` & `bo4e-202401.1.1rc4/src/bo4e/bo/preisblattdienstleistung.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/bo/preisblatthardware.py` & `bo4e-202401.1.1rc4/src/bo4e/bo/preisblatthardware.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/bo/preisblattkonzessionsabgabe.py` & `bo4e-202401.1.1rc4/src/bo4e/bo/preisblattkonzessionsabgabe.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/bo/preisblattmessung.py` & `bo4e-202401.1.1rc4/src/bo4e/bo/preisblattmessung.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/bo/preisblattnetznutzung.py` & `bo4e-202401.1.1rc4/src/bo4e/bo/preisblattnetznutzung.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/bo/rechnung.py` & `bo4e-202401.1.1rc4/src/bo4e/bo/rechnung.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/bo/region.py` & `bo4e-202401.1.1rc4/src/bo4e/bo/region.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/bo/regionaltarif.py` & `bo4e-202401.1.1rc4/src/bo4e/bo/regionaltarif.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/bo/standorteigenschaften.py` & `bo4e-202401.1.1rc4/src/bo4e/bo/standorteigenschaften.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/bo/tarif.py` & `bo4e-202401.1.1rc4/src/bo4e/bo/tarif.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/bo/tarifinfo.py` & `bo4e-202401.1.1rc4/src/bo4e/bo/tarifinfo.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/bo/tarifkosten.py` & `bo4e-202401.1.1rc4/src/bo4e/bo/tarifkosten.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/bo/tarifpreisblatt.py` & `bo4e-202401.1.1rc4/src/bo4e/bo/tarifpreisblatt.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/bo/vertrag.py` & `bo4e-202401.1.1rc4/src/bo4e/bo/vertrag.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/bo/zaehler.py` & `bo4e-202401.1.1rc4/src/bo4e/bo/zaehler.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/bo/zeitreihe.py` & `bo4e-202401.1.1rc4/src/bo4e/bo/zeitreihe.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/com/adresse.py` & `bo4e-202401.1.1rc4/src/bo4e/com/adresse.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/com/angebotsposition.py` & `bo4e-202401.1.1rc4/src/bo4e/com/angebotsposition.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/com/angebotsteil.py` & `bo4e-202401.1.1rc4/src/bo4e/com/angebotsteil.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/com/angebotsvariante.py` & `bo4e-202401.1.1rc4/src/bo4e/com/angebotsvariante.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/com/aufabschlag.py` & `bo4e-202401.1.1rc4/src/bo4e/com/aufabschlag.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/com/aufabschlagproort.py` & `bo4e-202401.1.1rc4/src/bo4e/com/aufabschlagproort.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/com/aufabschlagregional.py` & `bo4e-202401.1.1rc4/src/bo4e/com/aufabschlagregional.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/com/aufabschlagstaffelproort.py` & `bo4e-202401.1.1rc4/src/bo4e/com/aufabschlagstaffelproort.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/com/ausschreibungsdetail.py` & `bo4e-202401.1.1rc4/src/bo4e/com/ausschreibungsdetail.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/com/ausschreibungslos.py` & `bo4e-202401.1.1rc4/src/bo4e/com/ausschreibungslos.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/com/betrag.py` & `bo4e-202401.1.1rc4/src/bo4e/com/betrag.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/com/com.py` & `bo4e-202401.1.1rc4/src/bo4e/com/com.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/com/dienstleistung.py` & `bo4e-202401.1.1rc4/src/bo4e/com/dienstleistung.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/com/energieherkunft.py` & `bo4e-202401.1.1rc4/src/bo4e/com/energieherkunft.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/com/energiemix.py` & `bo4e-202401.1.1rc4/src/bo4e/com/energiemix.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/com/fremdkostenblock.py` & `bo4e-202401.1.1rc4/src/bo4e/com/fremdkostenblock.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/com/fremdkostenposition.py` & `bo4e-202401.1.1rc4/src/bo4e/com/fremdkostenposition.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/com/geokoordinaten.py` & `bo4e-202401.1.1rc4/src/bo4e/com/geokoordinaten.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/com/katasteradresse.py` & `bo4e-202401.1.1rc4/src/bo4e/com/katasteradresse.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/com/kontaktweg.py` & `bo4e-202401.1.1rc4/src/bo4e/com/kontaktweg.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/com/konzessionsabgabe.py` & `bo4e-202401.1.1rc4/src/bo4e/com/konzessionsabgabe.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/com/kostenblock.py` & `bo4e-202401.1.1rc4/src/bo4e/com/kostenblock.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/com/kostenposition.py` & `bo4e-202401.1.1rc4/src/bo4e/com/kostenposition.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/com/kriteriumwert.py` & `bo4e-202401.1.1rc4/src/bo4e/com/kriteriumwert.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/com/marktgebietinfo.py` & `bo4e-202401.1.1rc4/src/bo4e/com/marktgebietinfo.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/com/menge.py` & `bo4e-202401.1.1rc4/src/bo4e/com/menge.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/com/messlokationszuordnung.py` & `bo4e-202401.1.1rc4/src/bo4e/com/messlokationszuordnung.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/com/positionsaufabschlag.py` & `bo4e-202401.1.1rc4/src/bo4e/com/positionsaufabschlag.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/com/preis.py` & `bo4e-202401.1.1rc4/src/bo4e/com/preis.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/com/preisgarantie.py` & `bo4e-202401.1.1rc4/src/bo4e/com/preisgarantie.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/com/preisposition.py` & `bo4e-202401.1.1rc4/src/bo4e/com/preisposition.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/com/preisstaffel.py` & `bo4e-202401.1.1rc4/src/bo4e/com/preisstaffel.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/com/rechnungsposition.py` & `bo4e-202401.1.1rc4/src/bo4e/com/rechnungsposition.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/com/regionalegueltigkeit.py` & `bo4e-202401.1.1rc4/src/bo4e/com/regionalegueltigkeit.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/com/regionalepreisgarantie.py` & `bo4e-202401.1.1rc4/src/bo4e/com/regionalepreisgarantie.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/com/regionalepreisstaffel.py` & `bo4e-202401.1.1rc4/src/bo4e/com/regionalepreisstaffel.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/com/regionaleraufabschlag.py` & `bo4e-202401.1.1rc4/src/bo4e/com/regionaleraufabschlag.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/com/regionaletarifpreisposition.py` & `bo4e-202401.1.1rc4/src/bo4e/com/regionaletarifpreisposition.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/com/regionskriterium.py` & `bo4e-202401.1.1rc4/src/bo4e/com/regionskriterium.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/com/sigmoidparameter.py` & `bo4e-202401.1.1rc4/src/bo4e/com/sigmoidparameter.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/com/standorteigenschaftengas.py` & `bo4e-202401.1.1rc4/src/bo4e/com/standorteigenschaftengas.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/com/standorteigenschaftenstrom.py` & `bo4e-202401.1.1rc4/src/bo4e/com/standorteigenschaftenstrom.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/com/steuerbetrag.py` & `bo4e-202401.1.1rc4/src/bo4e/com/steuerbetrag.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/com/tarifberechnungsparameter.py` & `bo4e-202401.1.1rc4/src/bo4e/com/tarifberechnungsparameter.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/com/tarifeinschraenkung.py` & `bo4e-202401.1.1rc4/src/bo4e/com/tarifeinschraenkung.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/com/tarifpreis.py` & `bo4e-202401.1.1rc4/src/bo4e/com/tarifpreis.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/com/tarifpreisposition.py` & `bo4e-202401.1.1rc4/src/bo4e/com/tarifpreisposition.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/com/tarifpreispositionproort.py` & `bo4e-202401.1.1rc4/src/bo4e/com/tarifpreispositionproort.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/com/tarifpreisstaffelproort.py` & `bo4e-202401.1.1rc4/src/bo4e/com/tarifpreisstaffelproort.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/com/unterschrift.py` & `bo4e-202401.1.1rc4/src/bo4e/com/unterschrift.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/com/verbrauch.py` & `bo4e-202401.1.1rc4/src/bo4e/com/verbrauch.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/com/vertragskonditionen.py` & `bo4e-202401.1.1rc4/src/bo4e/com/vertragskonditionen.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/com/vertragsteil.py` & `bo4e-202401.1.1rc4/src/bo4e/com/vertragsteil.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/com/verwendungszweckpromarktrolle.py` & `bo4e-202401.1.1rc4/src/bo4e/com/verwendungszweckpromarktrolle.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/com/zaehlwerk.py` & `bo4e-202401.1.1rc4/src/bo4e/com/zaehlwerk.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/com/zaehlzeitregister.py` & `bo4e-202401.1.1rc4/src/bo4e/com/zaehlzeitregister.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/com/zeitraum.py` & `bo4e-202401.1.1rc4/src/bo4e/com/zeitraum.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/com/zeitreihenwert.py` & `bo4e-202401.1.1rc4/src/bo4e/com/zeitreihenwert.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/com/zeitspanne.py` & `bo4e-202401.1.1rc4/src/bo4e/com/zeitspanne.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/com/zustaendigkeit.py` & `bo4e-202401.1.1rc4/src/bo4e/com/zustaendigkeit.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/enum/abgabeart.py` & `bo4e-202401.1.1rc4/src/bo4e/enum/abgabeart.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/enum/angebotsstatus.py` & `bo4e-202401.1.1rc4/src/bo4e/enum/angebotsstatus.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/enum/artikelid.py` & `bo4e-202401.1.1rc4/src/bo4e/enum/artikelid.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/enum/aufabschlagsziel.py` & `bo4e-202401.1.1rc4/src/bo4e/enum/aufabschlagsziel.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/enum/ausschreibungsportal.py` & `bo4e-202401.1.1rc4/src/bo4e/enum/ausschreibungsportal.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/enum/bdewartikelnummer.py` & `bo4e-202401.1.1rc4/src/bo4e/enum/bdewartikelnummer.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/enum/bemessungsgroesse.py` & `bo4e-202401.1.1rc4/src/bo4e/enum/bemessungsgroesse.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/enum/bilanzierungsmethode.py` & `bo4e-202401.1.1rc4/src/bo4e/enum/bilanzierungsmethode.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/enum/dienstleistungstyp.py` & `bo4e-202401.1.1rc4/src/bo4e/enum/dienstleistungstyp.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/enum/erzeugungsart.py` & `bo4e-202401.1.1rc4/src/bo4e/enum/erzeugungsart.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/enum/gebiettyp.py` & `bo4e-202401.1.1rc4/src/bo4e/enum/gebiettyp.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/enum/geraeteklasse.py` & `bo4e-202401.1.1rc4/src/bo4e/enum/geraeteklasse.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/enum/geraetetyp.py` & `bo4e-202401.1.1rc4/src/bo4e/enum/geraetetyp.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/enum/gueltigkeitstyp.py` & `bo4e-202401.1.1rc4/src/bo4e/enum/gueltigkeitstyp.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/enum/kalkulationsmethode.py` & `bo4e-202401.1.1rc4/src/bo4e/enum/kalkulationsmethode.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/enum/kostenklasse.py` & `bo4e-202401.1.1rc4/src/bo4e/enum/kostenklasse.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/enum/kundengruppe.py` & `bo4e-202401.1.1rc4/src/bo4e/enum/kundengruppe.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/enum/kundengruppeka.py` & `bo4e-202401.1.1rc4/src/bo4e/enum/kundengruppeka.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/enum/kundentyp.py` & `bo4e-202401.1.1rc4/src/bo4e/enum/kundentyp.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/enum/leistungstyp.py` & `bo4e-202401.1.1rc4/src/bo4e/enum/leistungstyp.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/enum/marktrolle.py` & `bo4e-202401.1.1rc4/src/bo4e/enum/marktrolle.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/enum/mengeneinheit.py` & `bo4e-202401.1.1rc4/src/bo4e/enum/mengeneinheit.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/enum/messgroesse.py` & `bo4e-202401.1.1rc4/src/bo4e/enum/messgroesse.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/enum/messpreistyp.py` & `bo4e-202401.1.1rc4/src/bo4e/enum/messpreistyp.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/enum/messwertstatus.py` & `bo4e-202401.1.1rc4/src/bo4e/enum/messwertstatus.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/enum/messwertstatuszusatz.py` & `bo4e-202401.1.1rc4/src/bo4e/enum/messwertstatuszusatz.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/enum/netzebene.py` & `bo4e-202401.1.1rc4/src/bo4e/enum/netzebene.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/enum/netznutzungrechnungstyp.py` & `bo4e-202401.1.1rc4/src/bo4e/enum/netznutzungrechnungstyp.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/enum/oekolabel.py` & `bo4e-202401.1.1rc4/src/bo4e/enum/oekolabel.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/enum/oekozertifikat.py` & `bo4e-202401.1.1rc4/src/bo4e/enum/oekozertifikat.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/enum/preisgarantietyp.py` & `bo4e-202401.1.1rc4/src/bo4e/enum/preisgarantietyp.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/enum/preistyp.py` & `bo4e-202401.1.1rc4/src/bo4e/enum/preistyp.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/enum/rechnungslegung.py` & `bo4e-202401.1.1rc4/src/bo4e/enum/rechnungslegung.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/enum/rechnungsstatus.py` & `bo4e-202401.1.1rc4/src/bo4e/enum/rechnungsstatus.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/enum/rechnungstyp.py` & `bo4e-202401.1.1rc4/src/bo4e/enum/rechnungstyp.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/enum/regionskriteriumtyp.py` & `bo4e-202401.1.1rc4/src/bo4e/enum/regionskriteriumtyp.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/enum/steuerkennzeichen.py` & `bo4e-202401.1.1rc4/src/bo4e/enum/steuerkennzeichen.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/enum/tarifkalkulationsmethode.py` & `bo4e-202401.1.1rc4/src/bo4e/enum/tarifkalkulationsmethode.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/enum/tarifmerkmal.py` & `bo4e-202401.1.1rc4/src/bo4e/enum/tarifmerkmal.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/enum/themengebiet.py` & `bo4e-202401.1.1rc4/src/bo4e/enum/themengebiet.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/enum/typ.py` & `bo4e-202401.1.1rc4/src/bo4e/enum/typ.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/enum/vertragsart.py` & `bo4e-202401.1.1rc4/src/bo4e/enum/vertragsart.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/enum/vertragsstatus.py` & `bo4e-202401.1.1rc4/src/bo4e/enum/vertragsstatus.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/enum/verwendungszweck.py` & `bo4e-202401.1.1rc4/src/bo4e/enum/verwendungszweck.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/enum/voraussetzungen.py` & `bo4e-202401.1.1rc4/src/bo4e/enum/voraussetzungen.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/enum/waehrungscode.py` & `bo4e-202401.1.1rc4/src/bo4e/enum/waehrungscode.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/enum/zaehlergroesse.py` & `bo4e-202401.1.1rc4/src/bo4e/enum/zaehlergroesse.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/enum/zaehlertyp.py` & `bo4e-202401.1.1rc4/src/bo4e/enum/zaehlertyp.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/src/bo4e/utils/__init__.py` & `bo4e-202401.1.1rc4/src/bo4e/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/tests/serialization_helper.py` & `bo4e-202401.1.1rc4/tests/serialization_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """
 A module that simplifies assertions for json serialization
 """
 
+from __future__ import annotations
+
 from typing import Any, Dict, Optional, TypeVar
 
 from dictdiffer import diff  # type:ignore[import-not-found]
 from pydantic import BaseModel
 
 T = TypeVar("T", bound=BaseModel)
```

### Comparing `bo4e-202401.1.0rc2/tests/test_adresse.py` & `bo4e-202401.1.1rc4/tests/test_adresse.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/tests/test_angebot.py` & `bo4e-202401.1.1rc4/tests/test_angebot.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/tests/test_angebotsposition.py` & `bo4e-202401.1.1rc4/tests/test_angebotsposition.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/tests/test_angebotsteil.py` & `bo4e-202401.1.1rc4/tests/test_angebotsteil.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/tests/test_angebotsvariante.py` & `bo4e-202401.1.1rc4/tests/test_angebotsvariante.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/tests/test_aufabschlag.py` & `bo4e-202401.1.1rc4/tests/test_aufabschlag.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/tests/test_aufabschlagproort.py` & `bo4e-202401.1.1rc4/tests/test_aufabschlagproort.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/tests/test_aufabschlagregional.py` & `bo4e-202401.1.1rc4/tests/test_aufabschlagregional.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/tests/test_aufabschlagstaffelproort.py` & `bo4e-202401.1.1rc4/tests/test_aufabschlagstaffelproort.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/tests/test_ausschreibung.py` & `bo4e-202401.1.1rc4/tests/test_ausschreibung.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/tests/test_ausschreibungsdetail.py` & `bo4e-202401.1.1rc4/tests/test_ausschreibungsdetail.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/tests/test_ausschreibungslos.py` & `bo4e-202401.1.1rc4/tests/test_ausschreibungslos.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/tests/test_betrag.py` & `bo4e-202401.1.1rc4/tests/test_betrag.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/tests/test_buendelvertrag.py` & `bo4e-202401.1.1rc4/tests/test_buendelvertrag.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/tests/test_energieherkunft.py` & `bo4e-202401.1.1rc4/tests/test_energieherkunft.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/tests/test_energiemenge.py` & `bo4e-202401.1.1rc4/tests/test_energiemenge.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/tests/test_energiemix.py` & `bo4e-202401.1.1rc4/tests/test_energiemix.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/tests/test_enums.py` & `bo4e-202401.1.1rc4/tests/test_enums.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/tests/test_fremdkosten.py` & `bo4e-202401.1.1rc4/tests/test_fremdkosten.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/tests/test_fremdkostenblock.py` & `bo4e-202401.1.1rc4/tests/test_fremdkostenblock.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/tests/test_fremdkostenposition.py` & `bo4e-202401.1.1rc4/tests/test_fremdkostenposition.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/tests/test_geokoordinaten.py` & `bo4e-202401.1.1rc4/tests/test_geokoordinaten.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/tests/test_geraet.py` & `bo4e-202401.1.1rc4/tests/test_geraet.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/tests/test_geschaeftsobjekt.py` & `bo4e-202401.1.1rc4/tests/test_geschaeftsobjekt.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/tests/test_geschaeftspartner.py` & `bo4e-202401.1.1rc4/tests/test_geschaeftspartner.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/tests/test_katasteradresse.py` & `bo4e-202401.1.1rc4/tests/test_katasteradresse.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/tests/test_kontakt.py` & `bo4e-202401.1.1rc4/tests/test_kontakt.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/tests/test_kosten.py` & `bo4e-202401.1.1rc4/tests/test_kosten.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/tests/test_kostenblock.py` & `bo4e-202401.1.1rc4/tests/test_kostenblock.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/tests/test_kostenposition.py` & `bo4e-202401.1.1rc4/tests/test_kostenposition.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/tests/test_kriteriumswert.py` & `bo4e-202401.1.1rc4/tests/test_kriteriumswert.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/tests/test_lastgang.py` & `bo4e-202401.1.1rc4/tests/test_lastgang.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/tests/test_marktgebietinfo.py` & `bo4e-202401.1.1rc4/tests/test_marktgebietinfo.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/tests/test_marktlokation.py` & `bo4e-202401.1.1rc4/tests/test_marktlokation.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/tests/test_marktteilnehmer.py` & `bo4e-202401.1.1rc4/tests/test_marktteilnehmer.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/tests/test_menge.py` & `bo4e-202401.1.1rc4/tests/test_menge.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/tests/test_messlokation.py` & `bo4e-202401.1.1rc4/tests/test_messlokation.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/tests/test_messlokationszuordnung.py` & `bo4e-202401.1.1rc4/tests/test_messlokationszuordnung.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/tests/test_person.py` & `bo4e-202401.1.1rc4/tests/test_person.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/tests/test_positionsaufabschlag.py` & `bo4e-202401.1.1rc4/tests/test_positionsaufabschlag.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/tests/test_preis.py` & `bo4e-202401.1.1rc4/tests/test_preis.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/tests/test_preisblatt.py` & `bo4e-202401.1.1rc4/tests/test_preisblatt.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/tests/test_preisblatt_dienstleistung.py` & `bo4e-202401.1.1rc4/tests/test_preisblatt_dienstleistung.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/tests/test_preisblatt_hardware.py` & `bo4e-202401.1.1rc4/tests/test_preisblatt_hardware.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/tests/test_preisblatt_konzessionsabgabe.py` & `bo4e-202401.1.1rc4/tests/test_preisblatt_konzessionsabgabe.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/tests/test_preisblatt_messung.py` & `bo4e-202401.1.1rc4/tests/test_preisblatt_messung.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/tests/test_preisblattnetznutzung.py` & `bo4e-202401.1.1rc4/tests/test_preisblattnetznutzung.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/tests/test_preisgarantie.py` & `bo4e-202401.1.1rc4/tests/test_preisgarantie.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/tests/test_preisposition.py` & `bo4e-202401.1.1rc4/tests/test_preisposition.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/tests/test_preisstaffel.py` & `bo4e-202401.1.1rc4/tests/test_preisstaffel.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/tests/test_rechnung.py` & `bo4e-202401.1.1rc4/tests/test_rechnung.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/tests/test_rechnungsposition.py` & `bo4e-202401.1.1rc4/tests/test_rechnungsposition.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/tests/test_region.py` & `bo4e-202401.1.1rc4/tests/test_region.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/tests/test_regionalegueltigkeit.py` & `bo4e-202401.1.1rc4/tests/test_regionalegueltigkeit.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/tests/test_regionalepreisgarantie.py` & `bo4e-202401.1.1rc4/tests/test_regionalepreisgarantie.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/tests/test_regionalepreisstaffel.py` & `bo4e-202401.1.1rc4/tests/test_regionalepreisstaffel.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/tests/test_regionaleraufabschlag.py` & `bo4e-202401.1.1rc4/tests/test_regionaleraufabschlag.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/tests/test_regionaletarifpreisposition.py` & `bo4e-202401.1.1rc4/tests/test_regionaletarifpreisposition.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/tests/test_regionaltarif.py` & `bo4e-202401.1.1rc4/tests/test_regionaltarif.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/tests/test_regionskriterium.py` & `bo4e-202401.1.1rc4/tests/test_regionskriterium.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/tests/test_sigmoidparameter.py` & `bo4e-202401.1.1rc4/tests/test_sigmoidparameter.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/tests/test_standorteigenschaften.py` & `bo4e-202401.1.1rc4/tests/test_standorteigenschaften.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/tests/test_standorteigenschaftengas.py` & `bo4e-202401.1.1rc4/tests/test_standorteigenschaftengas.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/tests/test_standorteigenschaftenstrom.py` & `bo4e-202401.1.1rc4/tests/test_standorteigenschaftenstrom.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/tests/test_steuerbetrag.py` & `bo4e-202401.1.1rc4/tests/test_steuerbetrag.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/tests/test_tarif.py` & `bo4e-202401.1.1rc4/tests/test_tarif.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/tests/test_tarifberechnungsparameter.py` & `bo4e-202401.1.1rc4/tests/test_tarifberechnungsparameter.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/tests/test_tarifeinschraenkung.py` & `bo4e-202401.1.1rc4/tests/test_tarifeinschraenkung.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/tests/test_tarifinfo.py` & `bo4e-202401.1.1rc4/tests/test_tarifinfo.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/tests/test_tarifkosten.py` & `bo4e-202401.1.1rc4/tests/test_tarifkosten.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/tests/test_tarifpreis.py` & `bo4e-202401.1.1rc4/tests/test_tarifpreis.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/tests/test_tarifpreisblatt.py` & `bo4e-202401.1.1rc4/tests/test_tarifpreisblatt.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/tests/test_tarifpreisposition.py` & `bo4e-202401.1.1rc4/tests/test_tarifpreisposition.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/tests/test_tarifpreispositionproort.py` & `bo4e-202401.1.1rc4/tests/test_tarifpreispositionproort.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/tests/test_tarifpreisstaffelproort.py` & `bo4e-202401.1.1rc4/tests/test_tarifpreisstaffelproort.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/tests/test_unterschrift.py` & `bo4e-202401.1.1rc4/tests/test_unterschrift.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/tests/test_verbrauch.py` & `bo4e-202401.1.1rc4/tests/test_verbrauch.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/tests/test_vertrag.py` & `bo4e-202401.1.1rc4/tests/test_vertrag.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/tests/test_vertragskonditionen.py` & `bo4e-202401.1.1rc4/tests/test_vertragskonditionen.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/tests/test_vertragsteil.py` & `bo4e-202401.1.1rc4/tests/test_vertragsteil.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/tests/test_zaehler.py` & `bo4e-202401.1.1rc4/tests/test_zaehler.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/tests/test_zeitraum.py` & `bo4e-202401.1.1rc4/tests/test_zeitraum.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/tests/test_zeitreihe.py` & `bo4e-202401.1.1rc4/tests/test_zeitreihe.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/tests/test_zeitreihenwert.py` & `bo4e-202401.1.1rc4/tests/test_zeitreihenwert.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/tests/test_zeitspanne.py` & `bo4e-202401.1.1rc4/tests/test_zeitspanne.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/tests/test_zusatz_attribut.py` & `bo4e-202401.1.1rc4/tests/test_zusatz_attribut.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import pytest
 
 from bo4e import Anrede, Organisationstyp, Titel
 from bo4e.bo.geschaeftspartner import Geschaeftspartner
 from bo4e.bo.person import Person
 from bo4e.com.adresse import Adresse
 from bo4e.enum.geschaeftspartnerrolle import Geschaeftspartnerrolle
```

### Comparing `bo4e-202401.1.0rc2/tests/utils.py` & `bo4e-202401.1.1rc4/tests/utils.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/.gitignore` & `bo4e-202401.1.1rc4/.gitignore`

 * *Files 3% similar despite different names*

```diff
@@ -163,15 +163,18 @@
 Temporary Items
 .apdisk
 
 # This directory rebuilds on 'tox -e docs' therefore not needed in repo
 docs/api
 docs/plantuml.jar
 docs/_static/images
+docs/compatibility_matrix.csv
 
 # version number for bo4e-python; gets auto-generated during the command
 # python -m build
 src/_bo4e_python_version.py
 
 # the autogenerated JSON schemas will be build and pushed to BO4E-Schemas
 # on release
 json_schemas/**/*.json
+
+tmp/
```

### Comparing `bo4e-202401.1.0rc2/LICENSE.rst` & `bo4e-202401.1.1rc4/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc2/pyproject.toml` & `bo4e-202401.1.1rc4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["hatchling>=1.8.0", "hatch-vcs", "hatch-fancy-pypi-readme"]
 build-backend = "hatchling.build"
 
 [project]
 name = "bo4e"
 description = "Python Library that implements the BO4E Standard."
 license = { text = "MIT" }
-requires-python = ">=3.10"
+requires-python = ">=3.9"
 authors = [
   { name = "Kevin Krechan", email = "kevin.krechan@hochfrequenz.de" },
   { name = "Leon Haffmans", email = "leon.haffmans@hochfrequenz.de" },
   { name = "Annika Schlögl", email = "annika.schloegl@hochfrequenz.de" },
   { name = "Franziska Vesely", email = "franziska.vesely@hochfrequenz.de" },
   { name = "Konstantin Klein", email = "konstantin.klein@hochfrequenz.de" },
 ]
@@ -18,14 +18,15 @@
 classifiers = [
   "Development Status :: 4 - Beta",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3 :: Only",
+  "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
 ]
 # This list must be in synq with the ./requirements.in file!
 dependencies = ["iso3166", "pydantic>=2.0.0", "pyhumps"]
 dynamic = ["readme", "version"]
```

### Comparing `bo4e-202401.1.0rc2/PKG-INFO` & `bo4e-202401.1.1rc4/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: bo4e
-Version: 202401.1.0rc2
+Version: 202401.1.1rc4
 Summary: Python Library that implements the BO4E Standard.
 Project-URL: Changelog, https://github.com/bo4e/bo4e-python/releases
 Project-URL: Homepage, https://github.com/bo4e/bo4e-python
 Project-URL: Documentation, https://bo4e-python.readthedocs.io/en/latest/
 Author-email: Kevin Krechan <kevin.krechan@hochfrequenz.de>, Leon Haffmans <leon.haffmans@hochfrequenz.de>, Annika Schlögl <annika.schloegl@hochfrequenz.de>, Franziska Vesely <franziska.vesely@hochfrequenz.de>, Konstantin Klein <konstantin.klein@hochfrequenz.de>
 License: MIT
 License-File: AUTHORS.rst
@@ -12,18 +12,19 @@
 Keywords: bdew,bo4e,edi@energy
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.10
+Requires-Python: >=3.9
 Requires-Dist: iso3166
 Requires-Dist: pydantic>=2.0.0
 Requires-Dist: pyhumps
 Description-Content-Type: text/x-rst
 
 =============
 BO4E
@@ -75,15 +76,30 @@
 * Generell sollen Verweise zwischen zwei BOs bi-direktional sein, zwischen BOs und COMs aber nur unidirektional (z.B. soll jeder Zähler wissen zu welcher Messlokation er gehört aber eine Adresse muss nicht wissen, welchem Geschäftspartner, welcher Messlokation oder welcher Rechnung sie zugeordnet ist).
 * COMs können zwar weitere COMs beinhalten, jedoch sollte dies nicht dafür genutzt werden von einem COM eines BOs auf das COM eines anderen BOs zu verweisen.
   Bsp.: Die Adresse in Ansprechpartner ist identisch zur Lokationsadresse in der Marktlokation. Dann sollen beide Adressen als vollständiges COM dargestellt werden, statt nur als Verweis von einer Adresse auf die andere.
 * Oder anders formuliert: wir können aus einem BO oder einem COM auf ein anderes BO verweisen.
 
 Dokumentation / Fragen und Anregungen zum BO4E Datenmodell
 ==========================================================
-Eine Dokumentation des Datenmodells und JSON Schemata zur Erzeugung von Beispieldaten finden sich auf `read the docs <https://bo4e-python.readthedocs.io/en/latest/api/modules.html>`_.
+Die Dokumentation ist verfügbar unter `<https://bo4e.github.io/BO4E-python/>`_.
+Die Doku wird erst seit Version `v202401.0.3 <https://bo4e.github.io/BO4E-python/v202401.0.3>`_ mittels
+GitHub Pages gehosted.
+Die früheren Versionen sind auf `read the docs <https://bo4e-python.readthedocs.io/en/latest/api/modules.html>`_
+einsehbar.
+
+Unter `/latest` findet sich die Dokumentation des aktuellen Stands des main-Branches. `/stable` zeigt immer auf die
+letzte veröffentlichte Version (Release candidates ausgeschlossen).
+Zusätzlich ist jede Version (inklusive Release candidates) unter `/v<version>` auffindbar.
+
+Die Doku bietet eine Übersicht über alle Klassen und Attribute, die im BO4E Standard definiert sind. Außerdem
+werden alle Beziehungen zwischen den Klassen durch Diagramme visualisiert. Die JSON-Schemas sind ebenfalls verlinkt.
+Alternativ können die JSON-Schemas auch direkt von GitHub heruntergeladen werden: `<https://github.com/bo4e/BO4E-Schemas>`_.
+Seit Version `v202401.1.1 <https://bo4e.github.io/BO4E-python/v202401.1.1>`_ gibt es zusätzlich eine
+`Kompatibilitätsmatrix <https://bo4e.github.io/BO4E-python/v202401.1.1/changelog.html>`_,
+die für jedes Objekt zeigt, zwischen welchen Versionen es einen "breaking change" gab.
 
 Bei Fragen oder Anregungen, bitte `einfach ein Issue in diesem Repo aufmachen <https://github.com/Hochfrequenz/BO4E-python/issues/new?assignees=&labels=BO4E+Enhancement+Proposal&template=funktionale-anforderung-an-den-bo4e-standard.md&title=Ein+aussagekr%C3%A4ftiger+Titel%3A+Hunde-+und+Katzentarife+k%C3%B6nnen+nicht+abgebildet+werden>`_.
 
 Code Beiträge
 =============
 Änderungsvorschläge (sowohl an das Datenmodell als auch an die Implementierung in Python) können direkt als Code in Form von Pull Requests eingereicht werden.
 Details dazu finden sich im `Contribution Guide`_.
```

