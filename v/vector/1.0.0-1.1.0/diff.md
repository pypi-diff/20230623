# Comparing `tmp/vector-1.0.0.tar.gz` & `tmp/vector-1.1.0.tar.gz`

## Comparing `vector-1.0.0.tar` & `vector-1.1.0.tar`

### file list

```diff
@@ -1,306 +1,306 @@
--rw-r--r--   0        0        0     2354 2020-02-02 00:00:00.000000 vector-1.0.0/.all-contributorsrc
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 vector-1.0.0/.git_archival.txt
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 vector-1.0.0/.gitattributes
--rw-r--r--   0        0        0     2055 2020-02-02 00:00:00.000000 vector-1.0.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 vector-1.0.0/.readthedocs.yml
--rwxr-xr-x   0        0        0      887 2020-02-02 00:00:00.000000 vector-1.0.0/CITATION.cff
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 vector-1.0.0/environment.yml
--rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 vector-1.0.0/noxfile.py
--rw-r--r--   0        0        0     7045 2020-02-02 00:00:00.000000 vector-1.0.0/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 vector-1.0.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 vector-1.0.0/.github/codecov.yml
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 vector-1.0.0/.github/dependabot.yml
--rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 vector-1.0.0/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 vector-1.0.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 vector-1.0.0/.github/ISSUE_TEMPLATE/feature_request.yml
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 vector-1.0.0/.github/matchers/pylint.json
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 vector-1.0.0/.github/workflows/cd.yml
--rw-r--r--   0        0        0     4108 2020-02-02 00:00:00.000000 vector-1.0.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 vector-1.0.0/.github/workflows/notebooks.yml
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 vector-1.0.0/docs/Makefile
--rw-r--r--   0        0        0     9686 2020-02-02 00:00:00.000000 vector-1.0.0/docs/changelog.md
--rw-r--r--   0        0        0     3071 2020-02-02 00:00:00.000000 vector-1.0.0/docs/conf.py
--rw-r--r--   0        0        0     7931 2020-02-02 00:00:00.000000 vector-1.0.0/docs/index.rst
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 vector-1.0.0/docs/make.bat
--rw-r--r--   0        0        0     6473 2020-02-02 00:00:00.000000 vector-1.0.0/docs/_images/LogoSrc.svg
--rw-r--r--   0        0        0    12709 2020-02-02 00:00:00.000000 vector-1.0.0/docs/_images/vector-logo.png
--rw-r--r--   0        0        0   174177 2020-02-02 00:00:00.000000 vector-1.0.0/docs/api/inheritance.svg
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 vector-1.0.0/docs/api/modules.rst
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 vector-1.0.0/docs/api/vector._methods.rst
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 vector-1.0.0/docs/api/vector._typeutils.rst
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 vector-1.0.0/docs/api/vector.rst
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 vector-1.0.0/docs/api/vector.version.rst
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 vector-1.0.0/docs/api/backends/vector.backends._numba.rst
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 vector-1.0.0/docs/api/backends/vector.backends._numba_object.rst
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 vector-1.0.0/docs/api/backends/vector.backends.awkward.rst
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 vector-1.0.0/docs/api/backends/vector.backends.numba_numpy.rst
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 vector-1.0.0/docs/api/backends/vector.backends.numpy.rst
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 vector-1.0.0/docs/api/backends/vector.backends.object.rst
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 vector-1.0.0/docs/api/backends/vector.backends.rst
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 vector-1.0.0/docs/api/compute/vector._compute.rst
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 vector-1.0.0/docs/api/compute/lorentz/vector._compute.lorentz.Et.rst
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 vector-1.0.0/docs/api/compute/lorentz/vector._compute.lorentz.Et2.rst
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 vector-1.0.0/docs/api/compute/lorentz/vector._compute.lorentz.Mt.rst
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 vector-1.0.0/docs/api/compute/lorentz/vector._compute.lorentz.Mt2.rst
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 vector-1.0.0/docs/api/compute/lorentz/vector._compute.lorentz.add.rst
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 vector-1.0.0/docs/api/compute/lorentz/vector._compute.lorentz.beta.rst
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 vector-1.0.0/docs/api/compute/lorentz/vector._compute.lorentz.boostX_beta.rst
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 vector-1.0.0/docs/api/compute/lorentz/vector._compute.lorentz.boostX_gamma.rst
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 vector-1.0.0/docs/api/compute/lorentz/vector._compute.lorentz.boostY_beta.rst
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 vector-1.0.0/docs/api/compute/lorentz/vector._compute.lorentz.boostY_gamma.rst
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 vector-1.0.0/docs/api/compute/lorentz/vector._compute.lorentz.boostZ_beta.rst
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 vector-1.0.0/docs/api/compute/lorentz/vector._compute.lorentz.boostZ_gamma.rst
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 vector-1.0.0/docs/api/compute/lorentz/vector._compute.lorentz.boost_beta3.rst
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 vector-1.0.0/docs/api/compute/lorentz/vector._compute.lorentz.boost_p4.rst
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 vector-1.0.0/docs/api/compute/lorentz/vector._compute.lorentz.deltaRapidityPhi.rst
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 vector-1.0.0/docs/api/compute/lorentz/vector._compute.lorentz.deltaRapidityPhi2.rst
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 vector-1.0.0/docs/api/compute/lorentz/vector._compute.lorentz.dot.rst
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 vector-1.0.0/docs/api/compute/lorentz/vector._compute.lorentz.equal.rst
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 vector-1.0.0/docs/api/compute/lorentz/vector._compute.lorentz.gamma.rst
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 vector-1.0.0/docs/api/compute/lorentz/vector._compute.lorentz.is_lightlike.rst
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 vector-1.0.0/docs/api/compute/lorentz/vector._compute.lorentz.is_spacelike.rst
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 vector-1.0.0/docs/api/compute/lorentz/vector._compute.lorentz.is_timelike.rst
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 vector-1.0.0/docs/api/compute/lorentz/vector._compute.lorentz.isclose.rst
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 vector-1.0.0/docs/api/compute/lorentz/vector._compute.lorentz.not_equal.rst
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 vector-1.0.0/docs/api/compute/lorentz/vector._compute.lorentz.rapidity.rst
--rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 vector-1.0.0/docs/api/compute/lorentz/vector._compute.lorentz.rst
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 vector-1.0.0/docs/api/compute/lorentz/vector._compute.lorentz.scale.rst
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 vector-1.0.0/docs/api/compute/lorentz/vector._compute.lorentz.subtract.rst
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 vector-1.0.0/docs/api/compute/lorentz/vector._compute.lorentz.t.rst
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 vector-1.0.0/docs/api/compute/lorentz/vector._compute.lorentz.t2.rst
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 vector-1.0.0/docs/api/compute/lorentz/vector._compute.lorentz.tau.rst
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 vector-1.0.0/docs/api/compute/lorentz/vector._compute.lorentz.tau2.rst
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 vector-1.0.0/docs/api/compute/lorentz/vector._compute.lorentz.to_beta3.rst
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 vector-1.0.0/docs/api/compute/lorentz/vector._compute.lorentz.transform4D.rst
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 vector-1.0.0/docs/api/compute/lorentz/vector._compute.lorentz.unit.rst
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 vector-1.0.0/docs/api/compute/planar/vector._compute.planar.add.rst
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 vector-1.0.0/docs/api/compute/planar/vector._compute.planar.deltaphi.rst
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 vector-1.0.0/docs/api/compute/planar/vector._compute.planar.dot.rst
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 vector-1.0.0/docs/api/compute/planar/vector._compute.planar.equal.rst
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 vector-1.0.0/docs/api/compute/planar/vector._compute.planar.is_antiparallel.rst
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 vector-1.0.0/docs/api/compute/planar/vector._compute.planar.is_parallel.rst
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 vector-1.0.0/docs/api/compute/planar/vector._compute.planar.is_perpendicular.rst
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 vector-1.0.0/docs/api/compute/planar/vector._compute.planar.isclose.rst
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 vector-1.0.0/docs/api/compute/planar/vector._compute.planar.not_equal.rst
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 vector-1.0.0/docs/api/compute/planar/vector._compute.planar.phi.rst
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 vector-1.0.0/docs/api/compute/planar/vector._compute.planar.rho.rst
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 vector-1.0.0/docs/api/compute/planar/vector._compute.planar.rho2.rst
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 vector-1.0.0/docs/api/compute/planar/vector._compute.planar.rotateZ.rst
--rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 vector-1.0.0/docs/api/compute/planar/vector._compute.planar.rst
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 vector-1.0.0/docs/api/compute/planar/vector._compute.planar.scale.rst
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 vector-1.0.0/docs/api/compute/planar/vector._compute.planar.subtract.rst
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 vector-1.0.0/docs/api/compute/planar/vector._compute.planar.transform2D.rst
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 vector-1.0.0/docs/api/compute/planar/vector._compute.planar.unit.rst
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 vector-1.0.0/docs/api/compute/planar/vector._compute.planar.x.rst
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 vector-1.0.0/docs/api/compute/planar/vector._compute.planar.y.rst
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 vector-1.0.0/docs/api/compute/spatial/vector._compute.spatial.add.rst
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 vector-1.0.0/docs/api/compute/spatial/vector._compute.spatial.costheta.rst
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 vector-1.0.0/docs/api/compute/spatial/vector._compute.spatial.cottheta.rst
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 vector-1.0.0/docs/api/compute/spatial/vector._compute.spatial.cross.rst
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 vector-1.0.0/docs/api/compute/spatial/vector._compute.spatial.deltaR.rst
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 vector-1.0.0/docs/api/compute/spatial/vector._compute.spatial.deltaR2.rst
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 vector-1.0.0/docs/api/compute/spatial/vector._compute.spatial.deltaangle.rst
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 vector-1.0.0/docs/api/compute/spatial/vector._compute.spatial.deltaeta.rst
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 vector-1.0.0/docs/api/compute/spatial/vector._compute.spatial.dot.rst
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 vector-1.0.0/docs/api/compute/spatial/vector._compute.spatial.equal.rst
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 vector-1.0.0/docs/api/compute/spatial/vector._compute.spatial.eta.rst
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 vector-1.0.0/docs/api/compute/spatial/vector._compute.spatial.is_antiparallel.rst
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 vector-1.0.0/docs/api/compute/spatial/vector._compute.spatial.is_parallel.rst
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 vector-1.0.0/docs/api/compute/spatial/vector._compute.spatial.is_perpendicular.rst
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 vector-1.0.0/docs/api/compute/spatial/vector._compute.spatial.isclose.rst
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 vector-1.0.0/docs/api/compute/spatial/vector._compute.spatial.mag.rst
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 vector-1.0.0/docs/api/compute/spatial/vector._compute.spatial.mag2.rst
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 vector-1.0.0/docs/api/compute/spatial/vector._compute.spatial.not_equal.rst
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 vector-1.0.0/docs/api/compute/spatial/vector._compute.spatial.rotateX.rst
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 vector-1.0.0/docs/api/compute/spatial/vector._compute.spatial.rotateY.rst
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 vector-1.0.0/docs/api/compute/spatial/vector._compute.spatial.rotate_axis.rst
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 vector-1.0.0/docs/api/compute/spatial/vector._compute.spatial.rotate_euler.rst
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 vector-1.0.0/docs/api/compute/spatial/vector._compute.spatial.rotate_quaternion.rst
--rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 vector-1.0.0/docs/api/compute/spatial/vector._compute.spatial.rst
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 vector-1.0.0/docs/api/compute/spatial/vector._compute.spatial.scale.rst
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 vector-1.0.0/docs/api/compute/spatial/vector._compute.spatial.subtract.rst
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 vector-1.0.0/docs/api/compute/spatial/vector._compute.spatial.theta.rst
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 vector-1.0.0/docs/api/compute/spatial/vector._compute.spatial.transform3D.rst
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 vector-1.0.0/docs/api/compute/spatial/vector._compute.spatial.unit.rst
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 vector-1.0.0/docs/api/compute/spatial/vector._compute.spatial.z.rst
--rw-r--r--   0        0        0    72634 2020-02-02 00:00:00.000000 vector-1.0.0/docs/usage/intro.ipynb
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 vector-1.0.0/docs/usage/structure.md
--rw-r--r--   0        0        0     4359 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/__init__.py
--rw-r--r--   0        0        0   124263 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/_methods.py
--rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/_typeutils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/py.typed
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/version.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/version.pyi
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/_compute/__init__.py
--rw-r--r--   0        0        0     3355 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/_compute/lorentz/Et.py
--rw-r--r--   0        0        0     3397 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/_compute/lorentz/Et2.py
--rw-r--r--   0        0        0     3271 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/_compute/lorentz/Mt.py
--rw-r--r--   0        0        0     3398 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/_compute/lorentz/Mt2.py
--rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/_compute/lorentz/__init__.py
--rw-r--r--   0        0        0     7226 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/_compute/lorentz/add.py
--rw-r--r--   0        0        0     4280 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/_compute/lorentz/beta.py
--rw-r--r--   0        0        0     6277 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/_compute/lorentz/boostX_beta.py
--rw-r--r--   0        0        0     6637 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/_compute/lorentz/boostX_gamma.py
--rw-r--r--   0        0        0     6277 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/_compute/lorentz/boostY_beta.py
--rw-r--r--   0        0        0     6640 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/_compute/lorentz/boostY_gamma.py
--rw-r--r--   0        0        0     5685 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/_compute/lorentz/boostZ_beta.py
--rw-r--r--   0        0        0     6048 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/_compute/lorentz/boostZ_gamma.py
--rw-r--r--   0        0        0    10076 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/_compute/lorentz/boost_beta3.py
--rw-r--r--   0        0        0    21205 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/_compute/lorentz/boost_p4.py
--rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/_compute/lorentz/deltaRapidityPhi.py
--rw-r--r--   0        0        0     3279 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/_compute/lorentz/deltaRapidityPhi2.py
--rw-r--r--   0        0        0     5547 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/_compute/lorentz/dot.py
--rw-r--r--   0        0        0     5902 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/_compute/lorentz/equal.py
--rw-r--r--   0        0        0     4192 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/_compute/lorentz/gamma.py
--rw-r--r--   0        0        0     1998 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/_compute/lorentz/is_lightlike.py
--rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/_compute/lorentz/is_spacelike.py
--rw-r--r--   0        0        0     1953 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/_compute/lorentz/is_timelike.py
--rw-r--r--   0        0        0     6916 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/_compute/lorentz/isclose.py
--rw-r--r--   0        0        0     5906 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/_compute/lorentz/not_equal.py
--rw-r--r--   0        0        0     3653 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/_compute/lorentz/rapidity.py
--rw-r--r--   0        0        0     4885 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/_compute/lorentz/scale.py
--rw-r--r--   0        0        0     7256 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/_compute/lorentz/subtract.py
--rw-r--r--   0        0        0     2999 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/_compute/lorentz/t.py
--rw-r--r--   0        0        0     3417 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/_compute/lorentz/t2.py
--rw-r--r--   0        0        0     3357 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/_compute/lorentz/tau.py
--rw-r--r--   0        0        0     3088 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/_compute/lorentz/tau2.py
--rw-r--r--   0        0        0     4036 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/_compute/lorentz/to_beta3.py
--rw-r--r--   0        0        0     5848 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/_compute/lorentz/transform4D.py
--rw-r--r--   0        0        0     6681 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/_compute/lorentz/unit.py
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/_compute/planar/__init__.py
--rw-r--r--   0        0        0     1957 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/_compute/planar/add.py
--rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/_compute/planar/deltaphi.py
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/_compute/planar/dot.py
--rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/_compute/planar/equal.py
--rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/_compute/planar/is_antiparallel.py
--rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/_compute/planar/is_parallel.py
--rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/_compute/planar/is_perpendicular.py
--rw-r--r--   0        0        0     2465 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/_compute/planar/isclose.py
--rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/_compute/planar/not_equal.py
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/_compute/planar/phi.py
--rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/_compute/planar/rho.py
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/_compute/planar/rho2.py
--rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/_compute/planar/rotateZ.py
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/_compute/planar/scale.py
--rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/_compute/planar/subtract.py
--rw-r--r--   0        0        0     1421 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/_compute/planar/transform2D.py
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/_compute/planar/unit.py
--rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/_compute/planar/x.py
--rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/_compute/planar/y.py
--rw-r--r--   0        0        0     2277 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/_compute/spatial/__init__.py
--rw-r--r--   0        0        0    15729 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/_compute/spatial/add.py
--rw-r--r--   0        0        0     1975 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/_compute/spatial/costheta.py
--rw-r--r--   0        0        0     1987 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/_compute/spatial/cottheta.py
--rw-r--r--   0        0        0     4555 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/_compute/spatial/cross.py
--rw-r--r--   0        0        0    10974 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/_compute/spatial/deltaR.py
--rw-r--r--   0        0        0    13510 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/_compute/spatial/deltaR2.py
--rw-r--r--   0        0        0    14835 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/_compute/spatial/deltaangle.py
--rw-r--r--   0        0        0    10070 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/_compute/spatial/deltaeta.py
--rw-r--r--   0        0        0    15429 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/_compute/spatial/dot.py
--rw-r--r--   0        0        0    12703 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/_compute/spatial/equal.py
--rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/_compute/spatial/eta.py
--rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/_compute/spatial/is_antiparallel.py
--rw-r--r--   0        0        0     2509 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/_compute/spatial/is_parallel.py
--rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/_compute/spatial/is_perpendicular.py
--rw-r--r--   0        0        0    16523 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/_compute/spatial/isclose.py
--rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/_compute/spatial/mag.py
--rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/_compute/spatial/mag2.py
--rw-r--r--   0        0        0    12707 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/_compute/spatial/not_equal.py
--rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/_compute/spatial/rotateX.py
--rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/_compute/spatial/rotateY.py
--rw-r--r--   0        0        0     5104 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/_compute/spatial/rotate_axis.py
--rw-r--r--   0        0        0    10032 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/_compute/spatial/rotate_euler.py
--rw-r--r--   0        0        0     3635 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/_compute/spatial/rotate_quaternion.py
--rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/_compute/spatial/scale.py
--rw-r--r--   0        0        0    15754 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/_compute/spatial/subtract.py
--rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/_compute/spatial/theta.py
--rw-r--r--   0        0        0     3522 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/_compute/spatial/transform3D.py
--rw-r--r--   0        0        0     2906 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/_compute/spatial/unit.py
--rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/_compute/spatial/z.py
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/backends/__init__.py
--rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/backends/_numba.py
--rw-r--r--   0        0        0   117564 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/backends/_numba_object.py
--rw-r--r--   0        0        0    66921 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/backends/awkward.py
--rw-r--r--   0        0        0    14319 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/backends/awkward_constructors.py
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/backends/numba_numpy.py
--rw-r--r--   0        0        0    67258 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/backends/numpy.py
--rw-r--r--   0        0        0   101667 2020-02-02 00:00:00.000000 vector-1.0.0/src/vector/backends/object.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 vector-1.0.0/tests/__init__.py
--rw-r--r--   0        0        0    11464 2020-02-02 00:00:00.000000 vector-1.0.0/tests/test_compute_features.py
--rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 vector-1.0.0/tests/test_issues.py
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 vector-1.0.0/tests/test_methods.py
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 vector-1.0.0/tests/test_notebooks.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 vector-1.0.0/tests/backends/__init__.py
--rw-r--r--   0        0        0     8235 2020-02-02 00:00:00.000000 vector-1.0.0/tests/backends/test_awkward.py
--rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 vector-1.0.0/tests/backends/test_awkward_numba.py
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 vector-1.0.0/tests/backends/test_numba_numpy.py
--rw-r--r--   0        0        0    54479 2020-02-02 00:00:00.000000 vector-1.0.0/tests/backends/test_numba_object.py
--rw-r--r--   0        0        0     7791 2020-02-02 00:00:00.000000 vector-1.0.0/tests/backends/test_numpy.py
--rw-r--r--   0        0        0     7306 2020-02-02 00:00:00.000000 vector-1.0.0/tests/backends/test_object.py
--rw-r--r--   0        0        0     5101 2020-02-02 00:00:00.000000 vector-1.0.0/tests/backends/test_operators.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 vector-1.0.0/tests/compute/__init__.py
--rw-r--r--   0        0        0     7214 2020-02-02 00:00:00.000000 vector-1.0.0/tests/compute/test_add.py
--rw-r--r--   0        0        0    20389 2020-02-02 00:00:00.000000 vector-1.0.0/tests/compute/test_conversions.py
--rw-r--r--   0        0        0     5765 2020-02-02 00:00:00.000000 vector-1.0.0/tests/compute/test_dot.py
--rw-r--r--   0        0        0     5933 2020-02-02 00:00:00.000000 vector-1.0.0/tests/compute/test_equal.py
--rw-r--r--   0        0        0     5564 2020-02-02 00:00:00.000000 vector-1.0.0/tests/compute/test_isclose.py
--rw-r--r--   0        0        0     6005 2020-02-02 00:00:00.000000 vector-1.0.0/tests/compute/test_not_equal.py
--rw-r--r--   0        0        0    11075 2020-02-02 00:00:00.000000 vector-1.0.0/tests/compute/test_scale.py
--rw-r--r--   0        0        0     7263 2020-02-02 00:00:00.000000 vector-1.0.0/tests/compute/test_subtract.py
--rw-r--r--   0        0        0     5350 2020-02-02 00:00:00.000000 vector-1.0.0/tests/compute/test_unit.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 vector-1.0.0/tests/compute/lorentz/__init__.py
--rw-r--r--   0        0        0     4153 2020-02-02 00:00:00.000000 vector-1.0.0/tests/compute/lorentz/test_Et.py
--rw-r--r--   0        0        0     4020 2020-02-02 00:00:00.000000 vector-1.0.0/tests/compute/lorentz/test_Et2.py
--rw-r--r--   0        0        0     4165 2020-02-02 00:00:00.000000 vector-1.0.0/tests/compute/lorentz/test_Mt.py
--rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 vector-1.0.0/tests/compute/lorentz/test_Mt2.py
--rw-r--r--   0        0        0     4584 2020-02-02 00:00:00.000000 vector-1.0.0/tests/compute/lorentz/test_beta.py
--rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 vector-1.0.0/tests/compute/lorentz/test_boostX_beta.py
--rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 vector-1.0.0/tests/compute/lorentz/test_boostX_gamma.py
--rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 vector-1.0.0/tests/compute/lorentz/test_boostY_beta.py
--rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 vector-1.0.0/tests/compute/lorentz/test_boostY_gamma.py
--rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 vector-1.0.0/tests/compute/lorentz/test_boostZ_beta.py
--rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 vector-1.0.0/tests/compute/lorentz/test_boostZ_gamma.py
--rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 vector-1.0.0/tests/compute/lorentz/test_boost_beta3.py
--rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 vector-1.0.0/tests/compute/lorentz/test_boost_p4.py
--rw-r--r--   0        0        0     3350 2020-02-02 00:00:00.000000 vector-1.0.0/tests/compute/lorentz/test_deltaRapidityPhi.py
--rw-r--r--   0        0        0     3334 2020-02-02 00:00:00.000000 vector-1.0.0/tests/compute/lorentz/test_deltaRapidityPhi2.py
--rw-r--r--   0        0        0     4212 2020-02-02 00:00:00.000000 vector-1.0.0/tests/compute/lorentz/test_gamma.py
--rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 vector-1.0.0/tests/compute/lorentz/test_rapidity.py
--rw-r--r--   0        0        0     4356 2020-02-02 00:00:00.000000 vector-1.0.0/tests/compute/lorentz/test_t.py
--rw-r--r--   0        0        0     4380 2020-02-02 00:00:00.000000 vector-1.0.0/tests/compute/lorentz/test_t2.py
--rw-r--r--   0        0        0     4536 2020-02-02 00:00:00.000000 vector-1.0.0/tests/compute/lorentz/test_tau.py
--rw-r--r--   0        0        0     4404 2020-02-02 00:00:00.000000 vector-1.0.0/tests/compute/lorentz/test_tau2.py
--rw-r--r--   0        0        0     8220 2020-02-02 00:00:00.000000 vector-1.0.0/tests/compute/lorentz/test_to_beta3.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 vector-1.0.0/tests/compute/planar/__init__.py
--rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 vector-1.0.0/tests/compute/planar/test_deltaphi.py
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 vector-1.0.0/tests/compute/planar/test_phi.py
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 vector-1.0.0/tests/compute/planar/test_rho.py
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 vector-1.0.0/tests/compute/planar/test_rho2.py
--rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 vector-1.0.0/tests/compute/planar/test_rotateZ.py
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 vector-1.0.0/tests/compute/planar/test_x.py
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 vector-1.0.0/tests/compute/planar/test_y.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 vector-1.0.0/tests/compute/spatial/__init__.py
--rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 vector-1.0.0/tests/compute/spatial/test_costheta.py
--rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 vector-1.0.0/tests/compute/spatial/test_cottheta.py
--rw-r--r--   0        0        0     6730 2020-02-02 00:00:00.000000 vector-1.0.0/tests/compute/spatial/test_cross.py
--rw-r--r--   0        0        0     4825 2020-02-02 00:00:00.000000 vector-1.0.0/tests/compute/spatial/test_deltaR.py
--rw-r--r--   0        0        0     4732 2020-02-02 00:00:00.000000 vector-1.0.0/tests/compute/spatial/test_deltaR2.py
--rw-r--r--   0        0        0     4654 2020-02-02 00:00:00.000000 vector-1.0.0/tests/compute/spatial/test_deltaangle.py
--rw-r--r--   0        0        0     4748 2020-02-02 00:00:00.000000 vector-1.0.0/tests/compute/spatial/test_deltaeta.py
--rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 vector-1.0.0/tests/compute/spatial/test_eta.py
--rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 vector-1.0.0/tests/compute/spatial/test_mag.py
--rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 vector-1.0.0/tests/compute/spatial/test_mag2.py
--rw-r--r--   0        0        0     4843 2020-02-02 00:00:00.000000 vector-1.0.0/tests/compute/spatial/test_rotateX.py
--rw-r--r--   0        0        0     4859 2020-02-02 00:00:00.000000 vector-1.0.0/tests/compute/spatial/test_rotateY.py
--rw-r--r--   0        0        0     7697 2020-02-02 00:00:00.000000 vector-1.0.0/tests/compute/spatial/test_rotate_axis.py
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 vector-1.0.0/tests/compute/spatial/test_rotate_euler.py
--rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 vector-1.0.0/tests/compute/spatial/test_rotate_quaternion.py
--rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 vector-1.0.0/tests/compute/spatial/test_theta.py
--rw-r--r--   0        0        0     1904 2020-02-02 00:00:00.000000 vector-1.0.0/tests/compute/spatial/test_z.py
--rw-r--r--   0        0        0   235709 2020-02-02 00:00:00.000000 vector-1.0.0/tests/samples/issue-161-v2.pkl
--rw-r--r--   0        0        0   231208 2020-02-02 00:00:00.000000 vector-1.0.0/tests/samples/issue-161.pkl
--rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 vector-1.0.0/.gitignore
--rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 vector-1.0.0/LICENSE
--rw-r--r--   0        0        0    31389 2020-02-02 00:00:00.000000 vector-1.0.0/README.md
--rw-r--r--   0        0        0     5622 2020-02-02 00:00:00.000000 vector-1.0.0/pyproject.toml
--rw-r--r--   0        0        0    34317 2020-02-02 00:00:00.000000 vector-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     2354 2020-02-02 00:00:00.000000 vector-1.1.0/.all-contributorsrc
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 vector-1.1.0/.git_archival.txt
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 vector-1.1.0/.gitattributes
+-rw-r--r--   0        0        0     2067 2020-02-02 00:00:00.000000 vector-1.1.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 vector-1.1.0/.readthedocs.yml
+-rwxr-xr-x   0        0        0      887 2020-02-02 00:00:00.000000 vector-1.1.0/CITATION.cff
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 vector-1.1.0/environment.yml
+-rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 vector-1.1.0/noxfile.py
+-rw-r--r--   0        0        0     7045 2020-02-02 00:00:00.000000 vector-1.1.0/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 vector-1.1.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 vector-1.1.0/.github/codecov.yml
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 vector-1.1.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 vector-1.1.0/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 vector-1.1.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 vector-1.1.0/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 vector-1.1.0/.github/matchers/pylint.json
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 vector-1.1.0/.github/workflows/cd.yml
+-rw-r--r--   0        0        0     4054 2020-02-02 00:00:00.000000 vector-1.1.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 vector-1.1.0/.github/workflows/notebooks.yml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 vector-1.1.0/docs/Makefile
+-rw-r--r--   0        0        0    10226 2020-02-02 00:00:00.000000 vector-1.1.0/docs/changelog.md
+-rw-r--r--   0        0        0     3071 2020-02-02 00:00:00.000000 vector-1.1.0/docs/conf.py
+-rw-r--r--   0        0        0     8007 2020-02-02 00:00:00.000000 vector-1.1.0/docs/index.rst
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 vector-1.1.0/docs/make.bat
+-rw-r--r--   0        0        0     6473 2020-02-02 00:00:00.000000 vector-1.1.0/docs/_images/LogoSrc.svg
+-rw-r--r--   0        0        0    12709 2020-02-02 00:00:00.000000 vector-1.1.0/docs/_images/vector-logo.png
+-rw-r--r--   0        0        0   174177 2020-02-02 00:00:00.000000 vector-1.1.0/docs/api/inheritance.svg
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 vector-1.1.0/docs/api/modules.rst
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 vector-1.1.0/docs/api/vector._methods.rst
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 vector-1.1.0/docs/api/vector._typeutils.rst
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 vector-1.1.0/docs/api/vector.rst
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 vector-1.1.0/docs/api/vector.version.rst
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 vector-1.1.0/docs/api/backends/vector.backends._numba.rst
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 vector-1.1.0/docs/api/backends/vector.backends._numba_object.rst
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 vector-1.1.0/docs/api/backends/vector.backends.awkward.rst
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 vector-1.1.0/docs/api/backends/vector.backends.numba_numpy.rst
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 vector-1.1.0/docs/api/backends/vector.backends.numpy.rst
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 vector-1.1.0/docs/api/backends/vector.backends.object.rst
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 vector-1.1.0/docs/api/backends/vector.backends.rst
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 vector-1.1.0/docs/api/compute/vector._compute.rst
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 vector-1.1.0/docs/api/compute/lorentz/vector._compute.lorentz.Et.rst
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 vector-1.1.0/docs/api/compute/lorentz/vector._compute.lorentz.Et2.rst
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 vector-1.1.0/docs/api/compute/lorentz/vector._compute.lorentz.Mt.rst
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 vector-1.1.0/docs/api/compute/lorentz/vector._compute.lorentz.Mt2.rst
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 vector-1.1.0/docs/api/compute/lorentz/vector._compute.lorentz.add.rst
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 vector-1.1.0/docs/api/compute/lorentz/vector._compute.lorentz.beta.rst
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 vector-1.1.0/docs/api/compute/lorentz/vector._compute.lorentz.boostX_beta.rst
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 vector-1.1.0/docs/api/compute/lorentz/vector._compute.lorentz.boostX_gamma.rst
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 vector-1.1.0/docs/api/compute/lorentz/vector._compute.lorentz.boostY_beta.rst
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 vector-1.1.0/docs/api/compute/lorentz/vector._compute.lorentz.boostY_gamma.rst
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 vector-1.1.0/docs/api/compute/lorentz/vector._compute.lorentz.boostZ_beta.rst
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 vector-1.1.0/docs/api/compute/lorentz/vector._compute.lorentz.boostZ_gamma.rst
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 vector-1.1.0/docs/api/compute/lorentz/vector._compute.lorentz.boost_beta3.rst
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 vector-1.1.0/docs/api/compute/lorentz/vector._compute.lorentz.boost_p4.rst
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 vector-1.1.0/docs/api/compute/lorentz/vector._compute.lorentz.deltaRapidityPhi.rst
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 vector-1.1.0/docs/api/compute/lorentz/vector._compute.lorentz.deltaRapidityPhi2.rst
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 vector-1.1.0/docs/api/compute/lorentz/vector._compute.lorentz.dot.rst
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 vector-1.1.0/docs/api/compute/lorentz/vector._compute.lorentz.equal.rst
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 vector-1.1.0/docs/api/compute/lorentz/vector._compute.lorentz.gamma.rst
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 vector-1.1.0/docs/api/compute/lorentz/vector._compute.lorentz.is_lightlike.rst
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 vector-1.1.0/docs/api/compute/lorentz/vector._compute.lorentz.is_spacelike.rst
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 vector-1.1.0/docs/api/compute/lorentz/vector._compute.lorentz.is_timelike.rst
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 vector-1.1.0/docs/api/compute/lorentz/vector._compute.lorentz.isclose.rst
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 vector-1.1.0/docs/api/compute/lorentz/vector._compute.lorentz.not_equal.rst
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 vector-1.1.0/docs/api/compute/lorentz/vector._compute.lorentz.rapidity.rst
+-rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 vector-1.1.0/docs/api/compute/lorentz/vector._compute.lorentz.rst
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 vector-1.1.0/docs/api/compute/lorentz/vector._compute.lorentz.scale.rst
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 vector-1.1.0/docs/api/compute/lorentz/vector._compute.lorentz.subtract.rst
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 vector-1.1.0/docs/api/compute/lorentz/vector._compute.lorentz.t.rst
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 vector-1.1.0/docs/api/compute/lorentz/vector._compute.lorentz.t2.rst
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 vector-1.1.0/docs/api/compute/lorentz/vector._compute.lorentz.tau.rst
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 vector-1.1.0/docs/api/compute/lorentz/vector._compute.lorentz.tau2.rst
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 vector-1.1.0/docs/api/compute/lorentz/vector._compute.lorentz.to_beta3.rst
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 vector-1.1.0/docs/api/compute/lorentz/vector._compute.lorentz.transform4D.rst
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 vector-1.1.0/docs/api/compute/lorentz/vector._compute.lorentz.unit.rst
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 vector-1.1.0/docs/api/compute/planar/vector._compute.planar.add.rst
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 vector-1.1.0/docs/api/compute/planar/vector._compute.planar.deltaphi.rst
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 vector-1.1.0/docs/api/compute/planar/vector._compute.planar.dot.rst
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 vector-1.1.0/docs/api/compute/planar/vector._compute.planar.equal.rst
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 vector-1.1.0/docs/api/compute/planar/vector._compute.planar.is_antiparallel.rst
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 vector-1.1.0/docs/api/compute/planar/vector._compute.planar.is_parallel.rst
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 vector-1.1.0/docs/api/compute/planar/vector._compute.planar.is_perpendicular.rst
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 vector-1.1.0/docs/api/compute/planar/vector._compute.planar.isclose.rst
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 vector-1.1.0/docs/api/compute/planar/vector._compute.planar.not_equal.rst
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 vector-1.1.0/docs/api/compute/planar/vector._compute.planar.phi.rst
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 vector-1.1.0/docs/api/compute/planar/vector._compute.planar.rho.rst
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 vector-1.1.0/docs/api/compute/planar/vector._compute.planar.rho2.rst
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 vector-1.1.0/docs/api/compute/planar/vector._compute.planar.rotateZ.rst
+-rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 vector-1.1.0/docs/api/compute/planar/vector._compute.planar.rst
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 vector-1.1.0/docs/api/compute/planar/vector._compute.planar.scale.rst
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 vector-1.1.0/docs/api/compute/planar/vector._compute.planar.subtract.rst
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 vector-1.1.0/docs/api/compute/planar/vector._compute.planar.transform2D.rst
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 vector-1.1.0/docs/api/compute/planar/vector._compute.planar.unit.rst
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 vector-1.1.0/docs/api/compute/planar/vector._compute.planar.x.rst
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 vector-1.1.0/docs/api/compute/planar/vector._compute.planar.y.rst
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 vector-1.1.0/docs/api/compute/spatial/vector._compute.spatial.add.rst
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 vector-1.1.0/docs/api/compute/spatial/vector._compute.spatial.costheta.rst
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 vector-1.1.0/docs/api/compute/spatial/vector._compute.spatial.cottheta.rst
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 vector-1.1.0/docs/api/compute/spatial/vector._compute.spatial.cross.rst
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 vector-1.1.0/docs/api/compute/spatial/vector._compute.spatial.deltaR.rst
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 vector-1.1.0/docs/api/compute/spatial/vector._compute.spatial.deltaR2.rst
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 vector-1.1.0/docs/api/compute/spatial/vector._compute.spatial.deltaangle.rst
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 vector-1.1.0/docs/api/compute/spatial/vector._compute.spatial.deltaeta.rst
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 vector-1.1.0/docs/api/compute/spatial/vector._compute.spatial.dot.rst
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 vector-1.1.0/docs/api/compute/spatial/vector._compute.spatial.equal.rst
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 vector-1.1.0/docs/api/compute/spatial/vector._compute.spatial.eta.rst
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 vector-1.1.0/docs/api/compute/spatial/vector._compute.spatial.is_antiparallel.rst
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 vector-1.1.0/docs/api/compute/spatial/vector._compute.spatial.is_parallel.rst
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 vector-1.1.0/docs/api/compute/spatial/vector._compute.spatial.is_perpendicular.rst
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 vector-1.1.0/docs/api/compute/spatial/vector._compute.spatial.isclose.rst
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 vector-1.1.0/docs/api/compute/spatial/vector._compute.spatial.mag.rst
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 vector-1.1.0/docs/api/compute/spatial/vector._compute.spatial.mag2.rst
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 vector-1.1.0/docs/api/compute/spatial/vector._compute.spatial.not_equal.rst
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 vector-1.1.0/docs/api/compute/spatial/vector._compute.spatial.rotateX.rst
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 vector-1.1.0/docs/api/compute/spatial/vector._compute.spatial.rotateY.rst
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 vector-1.1.0/docs/api/compute/spatial/vector._compute.spatial.rotate_axis.rst
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 vector-1.1.0/docs/api/compute/spatial/vector._compute.spatial.rotate_euler.rst
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 vector-1.1.0/docs/api/compute/spatial/vector._compute.spatial.rotate_quaternion.rst
+-rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 vector-1.1.0/docs/api/compute/spatial/vector._compute.spatial.rst
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 vector-1.1.0/docs/api/compute/spatial/vector._compute.spatial.scale.rst
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 vector-1.1.0/docs/api/compute/spatial/vector._compute.spatial.subtract.rst
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 vector-1.1.0/docs/api/compute/spatial/vector._compute.spatial.theta.rst
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 vector-1.1.0/docs/api/compute/spatial/vector._compute.spatial.transform3D.rst
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 vector-1.1.0/docs/api/compute/spatial/vector._compute.spatial.unit.rst
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 vector-1.1.0/docs/api/compute/spatial/vector._compute.spatial.z.rst
+-rw-r--r--   0        0        0    72634 2020-02-02 00:00:00.000000 vector-1.1.0/docs/usage/intro.ipynb
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 vector-1.1.0/docs/usage/structure.md
+-rw-r--r--   0        0        0     4272 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/__init__.py
+-rw-r--r--   0        0        0   123905 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/_methods.py
+-rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/_typeutils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/py.typed
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/version.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/version.pyi
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/_compute/__init__.py
+-rw-r--r--   0        0        0     3355 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/_compute/lorentz/Et.py
+-rw-r--r--   0        0        0     3397 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/_compute/lorentz/Et2.py
+-rw-r--r--   0        0        0     3271 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/_compute/lorentz/Mt.py
+-rw-r--r--   0        0        0     3398 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/_compute/lorentz/Mt2.py
+-rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/_compute/lorentz/__init__.py
+-rw-r--r--   0        0        0     7226 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/_compute/lorentz/add.py
+-rw-r--r--   0        0        0     4280 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/_compute/lorentz/beta.py
+-rw-r--r--   0        0        0     6277 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/_compute/lorentz/boostX_beta.py
+-rw-r--r--   0        0        0     6637 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/_compute/lorentz/boostX_gamma.py
+-rw-r--r--   0        0        0     6277 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/_compute/lorentz/boostY_beta.py
+-rw-r--r--   0        0        0     6640 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/_compute/lorentz/boostY_gamma.py
+-rw-r--r--   0        0        0     5685 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/_compute/lorentz/boostZ_beta.py
+-rw-r--r--   0        0        0     6048 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/_compute/lorentz/boostZ_gamma.py
+-rw-r--r--   0        0        0    10076 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/_compute/lorentz/boost_beta3.py
+-rw-r--r--   0        0        0    21205 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/_compute/lorentz/boost_p4.py
+-rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/_compute/lorentz/deltaRapidityPhi.py
+-rw-r--r--   0        0        0     3279 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/_compute/lorentz/deltaRapidityPhi2.py
+-rw-r--r--   0        0        0     5547 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/_compute/lorentz/dot.py
+-rw-r--r--   0        0        0     5902 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/_compute/lorentz/equal.py
+-rw-r--r--   0        0        0     4192 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/_compute/lorentz/gamma.py
+-rw-r--r--   0        0        0     1998 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/_compute/lorentz/is_lightlike.py
+-rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/_compute/lorentz/is_spacelike.py
+-rw-r--r--   0        0        0     1953 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/_compute/lorentz/is_timelike.py
+-rw-r--r--   0        0        0     6916 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/_compute/lorentz/isclose.py
+-rw-r--r--   0        0        0     5906 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/_compute/lorentz/not_equal.py
+-rw-r--r--   0        0        0     3653 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/_compute/lorentz/rapidity.py
+-rw-r--r--   0        0        0     4885 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/_compute/lorentz/scale.py
+-rw-r--r--   0        0        0     7256 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/_compute/lorentz/subtract.py
+-rw-r--r--   0        0        0     2999 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/_compute/lorentz/t.py
+-rw-r--r--   0        0        0     3417 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/_compute/lorentz/t2.py
+-rw-r--r--   0        0        0     3357 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/_compute/lorentz/tau.py
+-rw-r--r--   0        0        0     3088 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/_compute/lorentz/tau2.py
+-rw-r--r--   0        0        0     4036 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/_compute/lorentz/to_beta3.py
+-rw-r--r--   0        0        0     5848 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/_compute/lorentz/transform4D.py
+-rw-r--r--   0        0        0     6681 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/_compute/lorentz/unit.py
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/_compute/planar/__init__.py
+-rw-r--r--   0        0        0     1957 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/_compute/planar/add.py
+-rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/_compute/planar/deltaphi.py
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/_compute/planar/dot.py
+-rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/_compute/planar/equal.py
+-rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/_compute/planar/is_antiparallel.py
+-rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/_compute/planar/is_parallel.py
+-rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/_compute/planar/is_perpendicular.py
+-rw-r--r--   0        0        0     2465 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/_compute/planar/isclose.py
+-rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/_compute/planar/not_equal.py
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/_compute/planar/phi.py
+-rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/_compute/planar/rho.py
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/_compute/planar/rho2.py
+-rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/_compute/planar/rotateZ.py
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/_compute/planar/scale.py
+-rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/_compute/planar/subtract.py
+-rw-r--r--   0        0        0     1421 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/_compute/planar/transform2D.py
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/_compute/planar/unit.py
+-rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/_compute/planar/x.py
+-rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/_compute/planar/y.py
+-rw-r--r--   0        0        0     2277 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/_compute/spatial/__init__.py
+-rw-r--r--   0        0        0    15729 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/_compute/spatial/add.py
+-rw-r--r--   0        0        0     1975 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/_compute/spatial/costheta.py
+-rw-r--r--   0        0        0     1987 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/_compute/spatial/cottheta.py
+-rw-r--r--   0        0        0     4555 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/_compute/spatial/cross.py
+-rw-r--r--   0        0        0    10974 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/_compute/spatial/deltaR.py
+-rw-r--r--   0        0        0    13510 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/_compute/spatial/deltaR2.py
+-rw-r--r--   0        0        0    14835 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/_compute/spatial/deltaangle.py
+-rw-r--r--   0        0        0    10070 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/_compute/spatial/deltaeta.py
+-rw-r--r--   0        0        0    15429 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/_compute/spatial/dot.py
+-rw-r--r--   0        0        0    12703 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/_compute/spatial/equal.py
+-rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/_compute/spatial/eta.py
+-rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/_compute/spatial/is_antiparallel.py
+-rw-r--r--   0        0        0     2509 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/_compute/spatial/is_parallel.py
+-rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/_compute/spatial/is_perpendicular.py
+-rw-r--r--   0        0        0    16523 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/_compute/spatial/isclose.py
+-rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/_compute/spatial/mag.py
+-rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/_compute/spatial/mag2.py
+-rw-r--r--   0        0        0    12707 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/_compute/spatial/not_equal.py
+-rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/_compute/spatial/rotateX.py
+-rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/_compute/spatial/rotateY.py
+-rw-r--r--   0        0        0     5104 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/_compute/spatial/rotate_axis.py
+-rw-r--r--   0        0        0    10032 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/_compute/spatial/rotate_euler.py
+-rw-r--r--   0        0        0     3635 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/_compute/spatial/rotate_quaternion.py
+-rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/_compute/spatial/scale.py
+-rw-r--r--   0        0        0    15754 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/_compute/spatial/subtract.py
+-rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/_compute/spatial/theta.py
+-rw-r--r--   0        0        0     3522 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/_compute/spatial/transform3D.py
+-rw-r--r--   0        0        0     2906 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/_compute/spatial/unit.py
+-rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/_compute/spatial/z.py
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/backends/__init__.py
+-rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/backends/_numba.py
+-rw-r--r--   0        0        0   116287 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/backends/_numba_object.py
+-rw-r--r--   0        0        0    68592 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/backends/awkward.py
+-rw-r--r--   0        0        0    14336 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/backends/awkward_constructors.py
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/backends/numba_numpy.py
+-rw-r--r--   0        0        0    69860 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/backends/numpy.py
+-rw-r--r--   0        0        0   101667 2020-02-02 00:00:00.000000 vector-1.1.0/src/vector/backends/object.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 vector-1.1.0/tests/__init__.py
+-rw-r--r--   0        0        0    11420 2020-02-02 00:00:00.000000 vector-1.1.0/tests/test_compute_features.py
+-rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 vector-1.1.0/tests/test_issues.py
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 vector-1.1.0/tests/test_methods.py
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 vector-1.1.0/tests/test_notebooks.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 vector-1.1.0/tests/backends/__init__.py
+-rw-r--r--   0        0        0    18760 2020-02-02 00:00:00.000000 vector-1.1.0/tests/backends/test_awkward.py
+-rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 vector-1.1.0/tests/backends/test_awkward_numba.py
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 vector-1.1.0/tests/backends/test_numba_numpy.py
+-rw-r--r--   0        0        0    54479 2020-02-02 00:00:00.000000 vector-1.1.0/tests/backends/test_numba_object.py
+-rw-r--r--   0        0        0    13986 2020-02-02 00:00:00.000000 vector-1.1.0/tests/backends/test_numpy.py
+-rw-r--r--   0        0        0     7306 2020-02-02 00:00:00.000000 vector-1.1.0/tests/backends/test_object.py
+-rw-r--r--   0        0        0     5101 2020-02-02 00:00:00.000000 vector-1.1.0/tests/backends/test_operators.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 vector-1.1.0/tests/compute/__init__.py
+-rw-r--r--   0        0        0     7214 2020-02-02 00:00:00.000000 vector-1.1.0/tests/compute/test_add.py
+-rw-r--r--   0        0        0    20389 2020-02-02 00:00:00.000000 vector-1.1.0/tests/compute/test_conversions.py
+-rw-r--r--   0        0        0     5765 2020-02-02 00:00:00.000000 vector-1.1.0/tests/compute/test_dot.py
+-rw-r--r--   0        0        0     5933 2020-02-02 00:00:00.000000 vector-1.1.0/tests/compute/test_equal.py
+-rw-r--r--   0        0        0     5564 2020-02-02 00:00:00.000000 vector-1.1.0/tests/compute/test_isclose.py
+-rw-r--r--   0        0        0     6005 2020-02-02 00:00:00.000000 vector-1.1.0/tests/compute/test_not_equal.py
+-rw-r--r--   0        0        0    11075 2020-02-02 00:00:00.000000 vector-1.1.0/tests/compute/test_scale.py
+-rw-r--r--   0        0        0     7263 2020-02-02 00:00:00.000000 vector-1.1.0/tests/compute/test_subtract.py
+-rw-r--r--   0        0        0     5350 2020-02-02 00:00:00.000000 vector-1.1.0/tests/compute/test_unit.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 vector-1.1.0/tests/compute/lorentz/__init__.py
+-rw-r--r--   0        0        0     4153 2020-02-02 00:00:00.000000 vector-1.1.0/tests/compute/lorentz/test_Et.py
+-rw-r--r--   0        0        0     4020 2020-02-02 00:00:00.000000 vector-1.1.0/tests/compute/lorentz/test_Et2.py
+-rw-r--r--   0        0        0     4165 2020-02-02 00:00:00.000000 vector-1.1.0/tests/compute/lorentz/test_Mt.py
+-rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 vector-1.1.0/tests/compute/lorentz/test_Mt2.py
+-rw-r--r--   0        0        0     4584 2020-02-02 00:00:00.000000 vector-1.1.0/tests/compute/lorentz/test_beta.py
+-rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 vector-1.1.0/tests/compute/lorentz/test_boostX_beta.py
+-rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 vector-1.1.0/tests/compute/lorentz/test_boostX_gamma.py
+-rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 vector-1.1.0/tests/compute/lorentz/test_boostY_beta.py
+-rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 vector-1.1.0/tests/compute/lorentz/test_boostY_gamma.py
+-rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 vector-1.1.0/tests/compute/lorentz/test_boostZ_beta.py
+-rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 vector-1.1.0/tests/compute/lorentz/test_boostZ_gamma.py
+-rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 vector-1.1.0/tests/compute/lorentz/test_boost_beta3.py
+-rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 vector-1.1.0/tests/compute/lorentz/test_boost_p4.py
+-rw-r--r--   0        0        0     3350 2020-02-02 00:00:00.000000 vector-1.1.0/tests/compute/lorentz/test_deltaRapidityPhi.py
+-rw-r--r--   0        0        0     3334 2020-02-02 00:00:00.000000 vector-1.1.0/tests/compute/lorentz/test_deltaRapidityPhi2.py
+-rw-r--r--   0        0        0     4212 2020-02-02 00:00:00.000000 vector-1.1.0/tests/compute/lorentz/test_gamma.py
+-rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 vector-1.1.0/tests/compute/lorentz/test_rapidity.py
+-rw-r--r--   0        0        0     4356 2020-02-02 00:00:00.000000 vector-1.1.0/tests/compute/lorentz/test_t.py
+-rw-r--r--   0        0        0     4380 2020-02-02 00:00:00.000000 vector-1.1.0/tests/compute/lorentz/test_t2.py
+-rw-r--r--   0        0        0     4536 2020-02-02 00:00:00.000000 vector-1.1.0/tests/compute/lorentz/test_tau.py
+-rw-r--r--   0        0        0     4404 2020-02-02 00:00:00.000000 vector-1.1.0/tests/compute/lorentz/test_tau2.py
+-rw-r--r--   0        0        0     8220 2020-02-02 00:00:00.000000 vector-1.1.0/tests/compute/lorentz/test_to_beta3.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 vector-1.1.0/tests/compute/planar/__init__.py
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 vector-1.1.0/tests/compute/planar/test_deltaphi.py
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 vector-1.1.0/tests/compute/planar/test_phi.py
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 vector-1.1.0/tests/compute/planar/test_rho.py
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 vector-1.1.0/tests/compute/planar/test_rho2.py
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 vector-1.1.0/tests/compute/planar/test_rotateZ.py
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 vector-1.1.0/tests/compute/planar/test_x.py
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 vector-1.1.0/tests/compute/planar/test_y.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 vector-1.1.0/tests/compute/spatial/__init__.py
+-rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 vector-1.1.0/tests/compute/spatial/test_costheta.py
+-rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 vector-1.1.0/tests/compute/spatial/test_cottheta.py
+-rw-r--r--   0        0        0     6730 2020-02-02 00:00:00.000000 vector-1.1.0/tests/compute/spatial/test_cross.py
+-rw-r--r--   0        0        0     4825 2020-02-02 00:00:00.000000 vector-1.1.0/tests/compute/spatial/test_deltaR.py
+-rw-r--r--   0        0        0     4732 2020-02-02 00:00:00.000000 vector-1.1.0/tests/compute/spatial/test_deltaR2.py
+-rw-r--r--   0        0        0     4654 2020-02-02 00:00:00.000000 vector-1.1.0/tests/compute/spatial/test_deltaangle.py
+-rw-r--r--   0        0        0     4748 2020-02-02 00:00:00.000000 vector-1.1.0/tests/compute/spatial/test_deltaeta.py
+-rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 vector-1.1.0/tests/compute/spatial/test_eta.py
+-rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 vector-1.1.0/tests/compute/spatial/test_mag.py
+-rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 vector-1.1.0/tests/compute/spatial/test_mag2.py
+-rw-r--r--   0        0        0     4843 2020-02-02 00:00:00.000000 vector-1.1.0/tests/compute/spatial/test_rotateX.py
+-rw-r--r--   0        0        0     4859 2020-02-02 00:00:00.000000 vector-1.1.0/tests/compute/spatial/test_rotateY.py
+-rw-r--r--   0        0        0     7697 2020-02-02 00:00:00.000000 vector-1.1.0/tests/compute/spatial/test_rotate_axis.py
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 vector-1.1.0/tests/compute/spatial/test_rotate_euler.py
+-rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 vector-1.1.0/tests/compute/spatial/test_rotate_quaternion.py
+-rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 vector-1.1.0/tests/compute/spatial/test_theta.py
+-rw-r--r--   0        0        0     1904 2020-02-02 00:00:00.000000 vector-1.1.0/tests/compute/spatial/test_z.py
+-rw-r--r--   0        0        0   235709 2020-02-02 00:00:00.000000 vector-1.1.0/tests/samples/issue-161-v2.pkl
+-rw-r--r--   0        0        0   231208 2020-02-02 00:00:00.000000 vector-1.1.0/tests/samples/issue-161.pkl
+-rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 vector-1.1.0/.gitignore
+-rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 vector-1.1.0/LICENSE
+-rw-r--r--   0        0        0    31461 2020-02-02 00:00:00.000000 vector-1.1.0/README.md
+-rw-r--r--   0        0        0     5370 2020-02-02 00:00:00.000000 vector-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0    34142 2020-02-02 00:00:00.000000 vector-1.1.0/PKG-INFO
```

### Comparing `vector-1.0.0/.all-contributorsrc` & `vector-1.1.0/.all-contributorsrc`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/.pre-commit-config.yaml` & `vector-1.1.0/.pre-commit-config.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ci:
   autoupdate_commit_msg: "chore: update pre-commit hooks"
   autofix_commit_msg: "style: pre-commit fixes"
 
 repos:
   - repo: https://github.com/psf/black
-    rev: 23.1.0
+    rev: 23.3.0
     hooks:
       - id: black-jupyter
 
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.4.0
     hooks:
       - id: check-added-large-files
@@ -20,48 +20,48 @@
       - id: end-of-file-fixer
         exclude: ^docs
       - id: mixed-line-ending
       - id: requirements-txt-fixer
       - id: trailing-whitespace
 
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: "v0.0.249"
+    rev: "v0.0.272"
     hooks:
       - id: ruff
         args: ["--fix", "--show-fixes"]
 
   - repo: https://github.com/tox-dev/pyproject-fmt
-    rev: "0.8.0"
+    rev: "0.12.0"
     hooks:
       - id: pyproject-fmt
 
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.0.1
+    rev: v1.3.0
     hooks:
       - id: mypy
         files: src
         args: []
         additional_dependencies:
           - numpy
           - packaging
 
   - repo: https://github.com/codespell-project/codespell
-    rev: v2.2.2
+    rev: v2.2.5
     hooks:
       - id: codespell
 
   - repo: https://github.com/pre-commit/mirrors-prettier
-    rev: "v3.0.0-alpha.4"
+    rev: "v3.0.0-alpha.9-for-vscode"
     hooks:
       - id: prettier
         types_or: [yaml, markdown, html, css, scss, javascript, json]
         exclude: assets/js/webapp\.js
 
   - repo: https://github.com/asottile/blacken-docs
-    rev: 1.13.0
+    rev: 1.14.0
     hooks:
       - id: blacken-docs
         args: ["-E"]
         additional_dependencies: [black==23.1.0]
 
   - repo: https://github.com/pre-commit/pygrep-hooks
     rev: v1.10.0
@@ -69,13 +69,13 @@
       - id: python-check-blanket-type-ignore
         exclude: ^src/vector/backends/_numba_object.py$
       - id: rst-backticks
       - id: rst-directive-colons
       - id: rst-inline-touching-normal
 
   - repo: https://github.com/nbQA-dev/nbQA
-    rev: 1.6.3
+    rev: 1.7.0
     hooks:
       - id: nbqa-pyupgrade
         args: ["--py37-plus"]
       - id: nbqa-isort
         args: ["--float-to-top"]
```

### Comparing `vector-1.0.0/CITATION.cff` & `vector-1.1.0/CITATION.cff`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/noxfile.py` & `vector-1.1.0/noxfile.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 from pathlib import Path
 
 import nox
 
-ALL_PYTHONS = ["3.7", "3.8", "3.9", "3.10", "3.11"]
+ALL_PYTHONS = ["3.8", "3.9", "3.10", "3.11"]
 
 nox.options.sessions = ["lint", "tests", "doctests"]
 
 
 DIR = Path(__file__).parent.resolve()
```

### Comparing `vector-1.0.0/.github/CONTRIBUTING.md` & `vector-1.1.0/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/.github/PULL_REQUEST_TEMPLATE.md` & `vector-1.1.0/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/.github/ISSUE_TEMPLATE/bug_report.yml` & `vector-1.1.0/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/.github/ISSUE_TEMPLATE/feature_request.yml` & `vector-1.1.0/.github/ISSUE_TEMPLATE/feature_request.yml`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/.github/matchers/pylint.json` & `vector-1.1.0/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/.github/workflows/cd.yml` & `vector-1.1.0/.github/workflows/cd.yml`

 * *Files 24% similar despite different names*

```diff
@@ -24,18 +24,20 @@
       - name: Check metadata
         run: pipx run twine check dist/*
 
   publish:
     needs: [dist]
     runs-on: ubuntu-latest
     if: github.event_name == 'release' && github.event.action == 'published'
+    environment:
+      name: pypi
+      url: https://pypi.org/p/vector
+    permissions:
+      id-token: write
 
     steps:
       - uses: actions/download-artifact@v3
         with:
           name: artifact
           path: dist
 
-      - uses: pypa/gh-action-pypi-publish@v1.6.4
-        with:
-          user: __token__
-          password: ${{ secrets.pypi_password }}
+      - uses: pypa/gh-action-pypi-publish@release/v1
```

### Comparing `vector-1.0.0/.github/workflows/ci.yml` & `vector-1.1.0/.github/workflows/ci.yml`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,14 @@
 
   check-light:
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
       matrix:
         python-version:
-          - "3.7"
           - "3.8"
           - "3.9"
           - "3.10"
           - "3.11"
     name: Python ${{ matrix.python-version }} - Light
     steps:
       - uses: actions/checkout@v3
@@ -60,15 +59,14 @@
   check-awkward-v1:
     needs: [check-light]
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
       matrix:
         python-version:
-          - "3.7"
           - "3.8"
           - "3.9"
           - "3.10"
           - "3.11"
     name: Python ${{ matrix.python-version }} - Awkward v1
     steps:
       - uses: actions/checkout@v3
@@ -92,15 +90,14 @@
   check-awkward-v2:
     needs: [check-light]
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
       matrix:
         python-version:
-          - "3.7"
           - "3.8"
           - "3.9"
           - "3.10"
           - "3.11"
     name: Python ${{ matrix.python-version }} - Awkward v2
     steps:
       - uses: actions/checkout@v3
@@ -118,15 +115,15 @@
       - name: Install awkward v2
         run: python -m pip install -U --pre "awkward>=2.0.0rc1"
 
       - name: Test package with awkward v2.x
         run: python -m pytest -ra --cov=vector --xdoctest --ignore tests/test_notebooks.py .
 
       - name: Upload coverage report
-        uses: codecov/codecov-action@v3.1.1
+        uses: codecov/codecov-action@v3.1.4
 
   discheck:
     runs-on: ubuntu-latest
     name: Disassemble check
     steps:
       - uses: actions/checkout@v3
```

### Comparing `vector-1.0.0/.github/workflows/notebooks.yml` & `vector-1.1.0/.github/workflows/notebooks.yml`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/docs/Makefile` & `vector-1.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/docs/changelog.md` & `vector-1.1.0/docs/changelog.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,28 @@
 # Changelog
 
+## Version 1.1
+
+### Version 1.1.0
+
+#### Features
+
+- feat: implement `sum`, `count`, and `count_nonzero` reductions [#347][]
+
+#### Maintenance
+
+- chore: remove Python `3.7` support [#355][]
+- chore: use trusted publisher deployment [#354][]
+- chore: replace custom definition of np.isclose with numba's np.isclose [#348][]
+
+[#355]: https://github.com/scikit-hep/vector/pull/355
+[#354]: https://github.com/scikit-hep/vector/pull/354
+[#347]: https://github.com/scikit-hep/vector/pull/347
+[#348]: https://github.com/scikit-hep/vector/pull/348
+
 ## Version 1.0
 
 ### Version 1.0.0
 
 #### Features
 
 - feat: add constructors for `VectorObject3D` and `MomentumObject3D` [#231][]
```

### Comparing `vector-1.0.0/docs/conf.py` & `vector-1.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/docs/index.rst` & `vector-1.1.0/docs/index.rst`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 |Action status| |Documentation Status| |pre-commit.ci status| |coverage| |GitHub Discussion| |Gitter| |Code style: black|
 
 |PyPI platforms| |PyPI version| |Conda latest releasetatus| |DOI| |License| |Scikit-HEP|
 
 Overview
 --------
 
-Vector is a Python 3.7+ library for 2D, 3D, and `Lorentz vectors <https://en.wikipedia.org/wiki/Special_relativity#Physics_in_spacetime>`_, especially *arrays of vectors*, to solve common physics problems in a NumPy-like way.
+Vector is a Python 3.8+ library (Python 3.6 and 3.7 supported till ``v0.9.0`` and ``v1.0.0``, respectively) for 2D, 3D, and `Lorentz vectors <https://en.wikipedia.org/wiki/Special_relativity#Physics_in_spacetime>`_, especially *arrays of vectors*, to solve common physics problems in a NumPy-like way.
 
 Main features of Vector:
 
 * Pure Python with NumPy as its only dependency. This makes it easier to install.
 * Vectors may be represented in a variety of coordinate systems: Cartesian, cylindrical, pseudorapidity, and any combination of these with time or proper time for Lorentz vectors. In all, there are 12 coordinate systems: {*x* - *y* vs *ρ* - *φ* in the azimuthal plane} × {*z* vs *θ* vs *η* longitudinally} × {*t* vs *τ* temporally}.
 * Uses names and conventions set by `ROOT <https://root.cern/>`_'s `TLorentzVector <https://root.cern.ch/doc/master/classTLorentzVector.html>`_ and `Math::LorentzVector <https://root.cern.ch/doc/master/classROOT_1_1Math_1_1LorentzVector.html>`_, as well as `scikit-hep/math <https://github.com/scikit-hep/scikit-hep/tree/master/skhep/math>`_, `uproot-methods TLorentzVector <https://github.com/scikit-hep/uproot3-methods/blob/master/uproot3_methods/classes/TLorentzVector.py>`_, `henryiii/hepvector <https://github.com/henryiii/hepvector>`_, and `coffea.nanoevents.methods.vector <https://coffeateam.github.io/coffea/modules/coffea.nanoevents.methods.vector.html>`_.
 * Implemented on a variety of backends:
```

### Comparing `vector-1.0.0/docs/make.bat` & `vector-1.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/docs/_images/LogoSrc.svg` & `vector-1.1.0/docs/_images/LogoSrc.svg`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/docs/_images/vector-logo.png` & `vector-1.1.0/docs/_images/vector-logo.png`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/docs/api/inheritance.svg` & `vector-1.1.0/docs/api/inheritance.svg`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/docs/api/compute/lorentz/vector._compute.lorentz.rst` & `vector-1.1.0/docs/api/compute/lorentz/vector._compute.lorentz.rst`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/docs/api/compute/planar/vector._compute.planar.rst` & `vector-1.1.0/docs/api/compute/planar/vector._compute.planar.rst`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/docs/api/compute/spatial/vector._compute.spatial.rst` & `vector-1.1.0/docs/api/compute/spatial/vector._compute.spatial.rst`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/docs/usage/intro.ipynb` & `vector-1.1.0/docs/usage/intro.ipynb`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/src/vector/__init__.py` & `vector-1.1.0/src/vector/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright (c) 2019-2023, Jonas Eschle, Jim Pivarski, Eduardo Rodrigues, and Henry Schreiner.
 #
 # Distributed under the 3-clause BSD license, see accompanying file LICENSE
 # or https://github.com/scikit-hep/vector for details.
 
 from __future__ import annotations
 
-import sys
+import importlib.metadata
 import typing
 
 import packaging.version
 
 from vector._methods import (
     Azimuthal,
     AzimuthalRhoPhi,
@@ -53,35 +53,30 @@
     VectorObject2D,
     VectorObject3D,
     VectorObject4D,
     obj,
 )
 from vector.version import version as __version__
 
-if sys.version_info < (3, 8):
-    import importlib_metadata
-else:
-    import importlib.metadata as importlib_metadata
-
 
 def _import_awkward() -> None:
-    awk_version = packaging.version.Version(importlib_metadata.version("awkward"))
+    awk_version = packaging.version.Version(importlib.metadata.version("awkward"))
     if awk_version < packaging.version.Version("1.2.0rc5"):
         # the only context users will see this message is if they're trying to use vector.awk
         # VectorAwkward is still set to None
         msg = f"awkward {awk_version} is too old; please upgrade to 1.2.0 or later"
         raise ImportError(msg)
 
 
 _is_awkward_v2: bool | None
 try:
     _is_awkward_v2 = packaging.version.Version(
-        importlib_metadata.version("awkward")
+        importlib.metadata.version("awkward")
     ) >= packaging.version.Version("2.0.0rc1")
-except importlib_metadata.PackageNotFoundError:
+except importlib.metadata.PackageNotFoundError:
     _is_awkward_v2 = None
 try:
     import awkward
 
     _import_awkward()
 except ImportError:
     awkward = None
@@ -174,10 +169,10 @@
     :func:`vector.Array` (or derived from such an array) have vector properties
     and methods.
     """
     import awkward
 
     import vector.backends.awkward
 
-    global _awkward_registered
+    global _awkward_registered  # noqa: PLW0603
     awkward.behavior.update(vector.backends.awkward.behavior)
     _awkward_registered = True
```

### Comparing `vector-1.0.0/src/vector/_methods.py` & `vector-1.1.0/src/vector/_methods.py`

 * *Files 1% similar despite different names*

```diff
@@ -3252,41 +3252,35 @@
 
         return scale.dispatch(factor, self)
 
     def equal(self, other: VectorProtocol) -> BoolCollection:
         from vector._compute.planar import equal
 
         if dim(self) != dim(other):
-            raise TypeError(
-                f"{repr(self)} and {repr(other)} do not have the same dimension"
-            )
+            raise TypeError(f"{self!r} and {other!r} do not have the same dimension")
         return equal.dispatch(self, other)
 
     def not_equal(self, other: VectorProtocol) -> BoolCollection:
         from vector._compute.planar import not_equal
 
         if dim(self) != dim(other):
-            raise TypeError(
-                f"{repr(self)} and {repr(other)} do not have the same dimension"
-            )
+            raise TypeError(f"{self!r} and {other!r} do not have the same dimension")
         return not_equal.dispatch(self, other)
 
     def isclose(
         self,
         other: VectorProtocol,
         rtol: ScalarCollection = 1e-05,
         atol: ScalarCollection = 1e-08,
         equal_nan: BoolCollection = False,
     ) -> BoolCollection:
         from vector._compute.planar import isclose
 
         if dim(self) != dim(other):
-            raise TypeError(
-                f"{repr(self)} and {repr(other)} do not have the same dimension"
-            )
+            raise TypeError(f"{self!r} and {other!r} do not have the same dimension")
         return isclose.dispatch(rtol, atol, equal_nan, self, other)
 
 
 class Spatial(Planar, VectorProtocolSpatial):
     @property
     def z(self) -> ScalarCollection:
         from vector._compute.spatial import z
@@ -3484,41 +3478,35 @@
 
         return scale.dispatch(factor, self)
 
     def equal(self, other: VectorProtocol) -> BoolCollection:
         from vector._compute.spatial import equal
 
         if dim(self) != dim(other):
-            raise TypeError(
-                f"{repr(self)} and {repr(other)} do not have the same dimension"
-            )
+            raise TypeError(f"{self!r} and {other!r} do not have the same dimension")
         return equal.dispatch(self, other)
 
     def not_equal(self, other: VectorProtocol) -> BoolCollection:
         from vector._compute.spatial import not_equal
 
         if dim(self) != dim(other):
-            raise TypeError(
-                f"{repr(self)} and {repr(other)} do not have the same dimension"
-            )
+            raise TypeError(f"{self!r} and {other!r} do not have the same dimension")
         return not_equal.dispatch(self, other)
 
     def isclose(
         self,
         other: VectorProtocol,
         rtol: ScalarCollection = 1e-05,
         atol: ScalarCollection = 1e-08,
         equal_nan: BoolCollection = False,
     ) -> BoolCollection:
         from vector._compute.spatial import isclose
 
         if dim(self) != dim(other):
-            raise TypeError(
-                f"{repr(self)} and {repr(other)} do not have the same dimension"
-            )
+            raise TypeError(f"{self!r} and {other!r} do not have the same dimension")
         return isclose.dispatch(rtol, atol, equal_nan, self, other)
 
 
 class Lorentz(Spatial, VectorProtocolLorentz):
     @property
     def t(self) -> ScalarCollection:
         from vector._compute.lorentz import t
@@ -3745,41 +3733,35 @@
 
         return scale.dispatch(factor, self)
 
     def equal(self, other: VectorProtocol) -> BoolCollection:
         from vector._compute.lorentz import equal
 
         if dim(self) != dim(other):
-            raise TypeError(
-                f"{repr(self)} and {repr(other)} do not have the same dimension"
-            )
+            raise TypeError(f"{self!r} and {other!r} do not have the same dimension")
         return equal.dispatch(self, other)
 
     def not_equal(self, other: VectorProtocol) -> BoolCollection:
         from vector._compute.lorentz import not_equal
 
         if dim(self) != dim(other):
-            raise TypeError(
-                f"{repr(self)} and {repr(other)} do not have the same dimension"
-            )
+            raise TypeError(f"{self!r} and {other!r} do not have the same dimension")
         return not_equal.dispatch(self, other)
 
     def isclose(
         self,
         other: VectorProtocol,
         rtol: ScalarCollection = 1e-05,
         atol: ScalarCollection = 1e-08,
         equal_nan: BoolCollection = False,
     ) -> BoolCollection:
         from vector._compute.lorentz import isclose
 
         if dim(self) != dim(other):
-            raise TypeError(
-                f"{repr(self)} and {repr(other)} do not have the same dimension"
-            )
+            raise TypeError(f"{self!r} and {other!r} do not have the same dimension")
         return isclose.dispatch(rtol, atol, equal_nan, self, other)
 
 
 class Momentum:
     pass
 
 
@@ -3938,30 +3920,30 @@
     if isinstance(v, Vector2D):
         return 2
     elif isinstance(v, Vector3D):
         return 3
     elif isinstance(v, Vector4D):
         return 4
     else:
-        raise TypeError(f"{repr(v)} is not a vector.Vector")
+        raise TypeError(f"{v!r} is not a vector.Vector")
 
 
 def _compute_module_of(
     one: VectorProtocol, two: VectorProtocol, nontemporal: bool = False
 ) -> Module:
     """
     Determines which compute module to use for functions of two vectors
     (the one with minimum dimension).
 
     If ``nontemporal``, use a spatial module even if both vectors are 4D.
     """
     if not isinstance(one, Vector):
-        raise TypeError(f"{repr(one)} is not a Vector")
+        raise TypeError(f"{one!r} is not a Vector")
     if not isinstance(two, Vector):
-        raise TypeError(f"{repr(two)} is not a Vector")
+        raise TypeError(f"{two!r} is not a Vector")
 
     if isinstance(one, Vector2D):
         import vector._compute.planar
 
         return vector._compute.planar
 
     elif isinstance(one, Vector3D):
@@ -4112,15 +4094,15 @@
     """
     Gets a function and its return type from a ``dispatch_map`` and the
     ``signature`` to search for (complaining if none is found).
     """
     result = dispatch_map.get(signature)
     if result is None:
         raise TypeError(
-            f"function {repr('.'.join(name.split('.')[-2:]))} has no signature {signature}"
+            f"function {'.'.join(name.split('.')[-2:])!r} has no signature {signature}"
         )
     return result
 
 
 _handler_priority = [
     "vector.backends.object",
     "vector.backends.numpy",
```

### Comparing `vector-1.0.0/src/vector/_typeutils.py` & `vector-1.1.0/src/vector/_typeutils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,16 @@
 # Copyright (c) 2019-2023, Jonas Eschle, Jim Pivarski, Eduardo Rodrigues, and Henry Schreiner.
 #
 # Distributed under the 3-clause BSD license, see accompanying file LICENSE
 # or https://github.com/scikit-hep/vector for details.
 
 from __future__ import annotations
 
-import sys
 import typing
-
-import numpy
-
-if sys.version_info < (3, 8):
-    from typing_extensions import Protocol, TypedDict
-else:
-    from typing import Protocol, TypedDict
-
+from typing import Protocol, TypedDict
 
 __all__ = [
     "Protocol",
     "ScalarCollection",
     "BoolCollection",
     "TransformProtocol2D",
     "TransformProtocol3D",
@@ -77,8 +69,10 @@
 
 
 if typing.TYPE_CHECKING:
     import numpy.typing
 
     FloatArray = numpy.typing.NDArray[numpy.float64]
 else:
+    import numpy
+
     FloatArray = numpy.ndarray
```

### Comparing `vector-1.0.0/src/vector/_compute/lorentz/Et.py` & `vector-1.1.0/src/vector/_compute/lorentz/Et.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/src/vector/_compute/lorentz/Et2.py` & `vector-1.1.0/src/vector/_compute/lorentz/Et2.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/src/vector/_compute/lorentz/Mt.py` & `vector-1.1.0/src/vector/_compute/lorentz/Mt.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/src/vector/_compute/lorentz/Mt2.py` & `vector-1.1.0/src/vector/_compute/lorentz/Mt2.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/src/vector/_compute/lorentz/__init__.py` & `vector-1.1.0/src/vector/_compute/lorentz/__init__.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/src/vector/_compute/lorentz/add.py` & `vector-1.1.0/src/vector/_compute/lorentz/add.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/src/vector/_compute/lorentz/beta.py` & `vector-1.1.0/src/vector/_compute/lorentz/beta.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/src/vector/_compute/lorentz/boostX_beta.py` & `vector-1.1.0/src/vector/_compute/lorentz/boostX_beta.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/src/vector/_compute/lorentz/boostX_gamma.py` & `vector-1.1.0/src/vector/_compute/lorentz/boostX_gamma.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/src/vector/_compute/lorentz/boostY_beta.py` & `vector-1.1.0/src/vector/_compute/lorentz/boostY_beta.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/src/vector/_compute/lorentz/boostY_gamma.py` & `vector-1.1.0/src/vector/_compute/lorentz/boostY_gamma.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/src/vector/_compute/lorentz/boostZ_beta.py` & `vector-1.1.0/src/vector/_compute/lorentz/boostZ_beta.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/src/vector/_compute/lorentz/boostZ_gamma.py` & `vector-1.1.0/src/vector/_compute/lorentz/boostZ_gamma.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/src/vector/_compute/lorentz/boost_beta3.py` & `vector-1.1.0/src/vector/_compute/lorentz/boost_beta3.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/src/vector/_compute/lorentz/boost_p4.py` & `vector-1.1.0/src/vector/_compute/lorentz/boost_p4.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/src/vector/_compute/lorentz/deltaRapidityPhi.py` & `vector-1.1.0/src/vector/_compute/lorentz/deltaRapidityPhi.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/src/vector/_compute/lorentz/deltaRapidityPhi2.py` & `vector-1.1.0/src/vector/_compute/lorentz/deltaRapidityPhi2.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/src/vector/_compute/lorentz/dot.py` & `vector-1.1.0/src/vector/_compute/lorentz/dot.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/src/vector/_compute/lorentz/equal.py` & `vector-1.1.0/src/vector/_compute/lorentz/equal.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/src/vector/_compute/lorentz/gamma.py` & `vector-1.1.0/src/vector/_compute/lorentz/gamma.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/src/vector/_compute/lorentz/is_lightlike.py` & `vector-1.1.0/src/vector/_compute/lorentz/is_lightlike.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/src/vector/_compute/lorentz/is_spacelike.py` & `vector-1.1.0/src/vector/_compute/lorentz/is_spacelike.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/src/vector/_compute/lorentz/is_timelike.py` & `vector-1.1.0/src/vector/_compute/lorentz/is_timelike.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/src/vector/_compute/lorentz/isclose.py` & `vector-1.1.0/src/vector/_compute/lorentz/isclose.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/src/vector/_compute/lorentz/not_equal.py` & `vector-1.1.0/src/vector/_compute/lorentz/not_equal.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/src/vector/_compute/lorentz/rapidity.py` & `vector-1.1.0/src/vector/_compute/lorentz/rapidity.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/src/vector/_compute/lorentz/scale.py` & `vector-1.1.0/src/vector/_compute/lorentz/scale.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/src/vector/_compute/lorentz/subtract.py` & `vector-1.1.0/src/vector/_compute/lorentz/subtract.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/src/vector/_compute/lorentz/t.py` & `vector-1.1.0/src/vector/_compute/lorentz/t.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/src/vector/_compute/lorentz/t2.py` & `vector-1.1.0/src/vector/_compute/lorentz/t2.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/src/vector/_compute/lorentz/tau.py` & `vector-1.1.0/src/vector/_compute/lorentz/tau.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/src/vector/_compute/lorentz/tau2.py` & `vector-1.1.0/src/vector/_compute/lorentz/tau2.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/src/vector/_compute/lorentz/to_beta3.py` & `vector-1.1.0/src/vector/_compute/lorentz/to_beta3.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/src/vector/_compute/lorentz/transform4D.py` & `vector-1.1.0/src/vector/_compute/lorentz/transform4D.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/src/vector/_compute/lorentz/unit.py` & `vector-1.1.0/src/vector/_compute/lorentz/unit.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/src/vector/_compute/planar/__init__.py` & `vector-1.1.0/src/vector/_compute/planar/__init__.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/src/vector/_compute/planar/add.py` & `vector-1.1.0/src/vector/_compute/planar/add.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/src/vector/_compute/planar/deltaphi.py` & `vector-1.1.0/src/vector/_compute/planar/deltaphi.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/src/vector/_compute/planar/dot.py` & `vector-1.1.0/src/vector/_compute/planar/dot.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/src/vector/_compute/planar/equal.py` & `vector-1.1.0/src/vector/_compute/planar/equal.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/src/vector/_compute/planar/is_antiparallel.py` & `vector-1.1.0/src/vector/_compute/planar/is_antiparallel.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/src/vector/_compute/planar/is_parallel.py` & `vector-1.1.0/src/vector/_compute/planar/is_parallel.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/src/vector/_compute/planar/is_perpendicular.py` & `vector-1.1.0/src/vector/_compute/planar/is_perpendicular.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/src/vector/_compute/planar/isclose.py` & `vector-1.1.0/src/vector/_compute/planar/isclose.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/src/vector/_compute/planar/not_equal.py` & `vector-1.1.0/src/vector/_compute/planar/not_equal.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/src/vector/_compute/planar/phi.py` & `vector-1.1.0/src/vector/_compute/planar/phi.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/src/vector/_compute/planar/rho.py` & `vector-1.1.0/src/vector/_compute/planar/rho.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/src/vector/_compute/planar/rho2.py` & `vector-1.1.0/src/vector/_compute/planar/rho2.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/src/vector/_compute/planar/rotateZ.py` & `vector-1.1.0/src/vector/_compute/planar/rotateZ.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/src/vector/_compute/planar/scale.py` & `vector-1.1.0/src/vector/_compute/planar/scale.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/src/vector/_compute/planar/subtract.py` & `vector-1.1.0/src/vector/_compute/planar/subtract.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/src/vector/_compute/planar/transform2D.py` & `vector-1.1.0/src/vector/_compute/planar/transform2D.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/src/vector/_compute/planar/unit.py` & `vector-1.1.0/src/vector/_compute/planar/unit.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/src/vector/_compute/planar/x.py` & `vector-1.1.0/src/vector/_compute/planar/x.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/src/vector/_compute/planar/y.py` & `vector-1.1.0/src/vector/_compute/planar/y.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/src/vector/_compute/spatial/__init__.py` & `vector-1.1.0/src/vector/_compute/spatial/__init__.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/src/vector/_compute/spatial/add.py` & `vector-1.1.0/src/vector/_compute/spatial/add.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/src/vector/_compute/spatial/costheta.py` & `vector-1.1.0/src/vector/_compute/spatial/costheta.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/src/vector/_compute/spatial/cottheta.py` & `vector-1.1.0/src/vector/_compute/spatial/cottheta.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/src/vector/_compute/spatial/cross.py` & `vector-1.1.0/src/vector/_compute/spatial/cross.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/src/vector/_compute/spatial/deltaR.py` & `vector-1.1.0/src/vector/_compute/spatial/deltaR.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/src/vector/_compute/spatial/deltaR2.py` & `vector-1.1.0/src/vector/_compute/spatial/deltaR2.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/src/vector/_compute/spatial/deltaangle.py` & `vector-1.1.0/src/vector/_compute/spatial/deltaangle.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/src/vector/_compute/spatial/deltaeta.py` & `vector-1.1.0/src/vector/_compute/spatial/deltaeta.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/src/vector/_compute/spatial/dot.py` & `vector-1.1.0/src/vector/_compute/spatial/dot.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/src/vector/_compute/spatial/equal.py` & `vector-1.1.0/src/vector/_compute/spatial/equal.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/src/vector/_compute/spatial/eta.py` & `vector-1.1.0/src/vector/_compute/spatial/eta.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/src/vector/_compute/spatial/is_antiparallel.py` & `vector-1.1.0/src/vector/_compute/spatial/is_antiparallel.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/src/vector/_compute/spatial/is_parallel.py` & `vector-1.1.0/src/vector/_compute/spatial/is_parallel.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/src/vector/_compute/spatial/is_perpendicular.py` & `vector-1.1.0/src/vector/_compute/spatial/is_perpendicular.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/src/vector/_compute/spatial/isclose.py` & `vector-1.1.0/src/vector/_compute/spatial/isclose.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/src/vector/_compute/spatial/mag.py` & `vector-1.1.0/src/vector/_compute/spatial/mag.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/src/vector/_compute/spatial/mag2.py` & `vector-1.1.0/src/vector/_compute/spatial/mag2.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/src/vector/_compute/spatial/not_equal.py` & `vector-1.1.0/src/vector/_compute/spatial/not_equal.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/src/vector/_compute/spatial/rotateX.py` & `vector-1.1.0/src/vector/_compute/spatial/rotateX.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/src/vector/_compute/spatial/rotateY.py` & `vector-1.1.0/src/vector/_compute/spatial/rotateY.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/src/vector/_compute/spatial/rotate_axis.py` & `vector-1.1.0/src/vector/_compute/spatial/rotate_axis.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/src/vector/_compute/spatial/rotate_euler.py` & `vector-1.1.0/src/vector/_compute/spatial/rotate_euler.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/src/vector/_compute/spatial/rotate_quaternion.py` & `vector-1.1.0/src/vector/_compute/spatial/rotate_quaternion.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/src/vector/_compute/spatial/scale.py` & `vector-1.1.0/src/vector/_compute/spatial/scale.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/src/vector/_compute/spatial/subtract.py` & `vector-1.1.0/src/vector/_compute/spatial/subtract.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/src/vector/_compute/spatial/theta.py` & `vector-1.1.0/src/vector/_compute/spatial/theta.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/src/vector/_compute/spatial/transform3D.py` & `vector-1.1.0/src/vector/_compute/spatial/transform3D.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/src/vector/_compute/spatial/unit.py` & `vector-1.1.0/src/vector/_compute/spatial/unit.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/src/vector/_compute/spatial/z.py` & `vector-1.1.0/src/vector/_compute/spatial/z.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/src/vector/backends/__init__.py` & `vector-1.1.0/src/vector/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/src/vector/backends/_numba.py` & `vector-1.1.0/src/vector/backends/_numba.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/src/vector/backends/_numba_object.py` & `vector-1.1.0/src/vector/backends/_numba_object.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,47 +90,14 @@
             if neginf is not None and numpy.isinf(x) and x < 0:
                 return neginf
             return x
 
     return nan_to_num_impl
 
 
-@numba.extending.overload(numpy.isclose)  # FIXME: This needs to go into Numba!
-def isclose(a, b, rtol=1e-05, atol=1e-08, equal_nan=False):
-    if isinstance(a, numba.types.Array) and isinstance(b, numba.types.Array):
-
-        def isclose_impl(a, b, rtol=1e-05, atol=1e-08, equal_nan=False):
-            a, b = numpy.broadcast_arrays(a, b)
-            x = a.reshape(-1)
-            y = b.astype(numpy.float64).reshape(-1)
-            out = numpy.zeros(len(x), numpy.bool_)
-            for i in range(len(out)):
-                if numpy.isnan(x[i]) and numpy.isnan(y[i]):
-                    out[i] = equal_nan
-                elif numpy.isinf(x[i]) and numpy.isinf(y[i]):
-                    out[i] = (x[i] > 0) == (y[i] > 0)
-                else:
-                    out[i] = abs(x[i] - y[i]) <= atol + rtol * abs(y[i])
-            return out.reshape(a.shape)
-
-    else:
-
-        def isclose_impl(a, b, rtol=1e-05, atol=1e-08, equal_nan=False):
-            x = a
-            y = numpy.float64(b)
-            if numpy.isnan(x) and numpy.isnan(y):
-                return equal_nan
-            elif numpy.isinf(x) and numpy.isinf(y):
-                return (x > 0) == (y > 0)
-            else:
-                return abs(x - y) <= atol + rtol * abs(y)
-
-    return isclose_impl
-
-
 # Since CoordinateObjects are NamedTuples, we get their types wrapped for free.
 
 
 def is_azimuthaltype(typ):
     return isinstance(
         typ, (numba.types.NamedTuple, numba.types.NamedUniTuple)
     ) and issubclass(typ.instance_class, AzimuthalObject)
```

### Comparing `vector-1.0.0/src/vector/backends/awkward.py` & `vector-1.1.0/src/vector/backends/awkward.py`

 * *Files 2% similar despite different names*

```diff
@@ -1611,15 +1611,15 @@
         awkwardtype,
         ak._connect.numba.layout.IndexedArrayType
         if hasattr(ak._connect, "numba")  # Awkward v2
         else ak._connect._numba.layout.IndexedArrayType,
     ):
         return _arraytype_of(awkwardtype.contenttype, component)
     raise numba.TypingError(
-        f"vector components like {repr(component)} must be NumpyArrayType, not {awkwardtype}"
+        f"vector components like {component!r} must be NumpyArrayType, not {awkwardtype}"
     )
 
 
 def _aztype_of(recordarraytype: typing.Any, is_momentum: bool) -> typing.Any:
     import numba
 
     cls: type[AzimuthalObjectXY] | type[AzimuthalObjectRhoPhi]
@@ -1974,20 +1974,89 @@
 
         def impl(record: typing.Any) -> typing.Any:
             return vectorcls(azimuthal(record), longitudinal(record), temporal(record))
 
     return context.compile_internal(builder, impl, sig, args)
 
 
-ak.behavior["__numba_typer__", "Vector2D"] = _numba_typer_Vector2D
-ak.behavior["__numba_typer__", "Vector3D"] = _numba_typer_Vector3D
-ak.behavior["__numba_typer__", "Vector4D"] = _numba_typer_Vector4D
-ak.behavior["__numba_typer__", "Momentum2D"] = _numba_typer_Momentum2D
-ak.behavior["__numba_typer__", "Momentum3D"] = _numba_typer_Momentum3D
-ak.behavior["__numba_typer__", "Momentum4D"] = _numba_typer_Momentum4D
-
-ak.behavior["__numba_lower__", "Vector2D"] = _numba_lower
-ak.behavior["__numba_lower__", "Vector3D"] = _numba_lower
-ak.behavior["__numba_lower__", "Vector4D"] = _numba_lower
-ak.behavior["__numba_lower__", "Momentum2D"] = _numba_lower
-ak.behavior["__numba_lower__", "Momentum3D"] = _numba_lower
-ak.behavior["__numba_lower__", "Momentum4D"] = _numba_lower
+behavior["__numba_typer__", "Vector2D"] = _numba_typer_Vector2D
+behavior["__numba_typer__", "Vector3D"] = _numba_typer_Vector3D
+behavior["__numba_typer__", "Vector4D"] = _numba_typer_Vector4D
+behavior["__numba_typer__", "Momentum2D"] = _numba_typer_Momentum2D
+behavior["__numba_typer__", "Momentum3D"] = _numba_typer_Momentum3D
+behavior["__numba_typer__", "Momentum4D"] = _numba_typer_Momentum4D
+
+behavior["__numba_lower__", "Vector2D"] = _numba_lower
+behavior["__numba_lower__", "Vector3D"] = _numba_lower
+behavior["__numba_lower__", "Vector4D"] = _numba_lower
+behavior["__numba_lower__", "Momentum2D"] = _numba_lower
+behavior["__numba_lower__", "Momentum3D"] = _numba_lower
+behavior["__numba_lower__", "Momentum4D"] = _numba_lower
+
+
+def _reduce_sum(
+    array: VectorArray2D
+    | VectorArray3D
+    | VectorArray4D
+    | MomentumArray2D
+    | MomentumArray3D
+    | MomentumArray4D,
+    mask_identity: bool,
+) -> VectorProtocol:
+    fields = {}
+    if isinstance(array, Lorentz):
+        fields["t"] = numpy.sum(array.t, axis=1)
+    if isinstance(array, Spatial):
+        fields["z"] = numpy.sum(array.z, axis=1)
+
+    assert isinstance(array, Planar)
+    fields["x"] = numpy.sum(array.x, axis=1)
+    fields["y"] = numpy.sum(array.y, axis=1)
+
+    layout = ak.to_layout(array)
+
+    return ak.zip(
+        fields,
+        behavior=array.behavior,
+        with_name=layout.purelist_parameter("__record__"),
+    )
+
+
+def _reduce_count(
+    array: VectorArray2D
+    | VectorArray3D
+    | VectorArray4D
+    | MomentumArray2D
+    | MomentumArray3D
+    | MomentumArray4D,
+    mask_identity: bool,
+) -> VectorProtocol:
+    first_field = array[array.fields[0]]
+    return ak.count(first_field, axis=1)
+
+
+def _reduce_count_nonzero(
+    array: VectorArray2D
+    | VectorArray3D
+    | VectorArray4D
+    | MomentumArray2D
+    | MomentumArray3D
+    | MomentumArray4D,
+    mask_identity: bool,
+) -> ScalarCollection:
+    is_nonzero = array.rho2 != 0
+    if isinstance(array, Spatial):
+        is_nonzero = numpy.logical_or(is_nonzero, array.z != 0)
+    if isinstance(array, Lorentz):
+        is_nonzero = numpy.logical_or(is_nonzero, array.t2 != 0)
+
+    return ak.count_nonzero(is_nonzero, axis=1)
+
+
+for reducer, impl in (
+    (ak.sum, _reduce_sum),
+    (ak.count, _reduce_count),
+    (ak.count_nonzero, _reduce_count_nonzero),
+):
+    for dim in range(2, 5):
+        behavior[reducer, f"Vector{dim}D"] = impl
+        behavior[reducer, f"Momentum{dim}D"] = impl
```

### Comparing `vector-1.0.0/src/vector/backends/awkward_constructors.py` & `vector-1.1.0/src/vector/backends/awkward_constructors.py`

 * *Files 1% similar despite different names*

```diff
@@ -226,15 +226,15 @@
 
     # .contents is Awkward v2
     contents = (
         array_type.contents if hasattr(array_type, "contents") else array_type.fields()
     )
     for field_type in contents:
         if isinstance(field_type, awkward.types.OptionType):
-            field_type = (
+            field_type = (  # noqa: PLW2901
                 field_type.content
                 if hasattr(array_type, "content")
                 else field_type.type
             )
         if not isinstance(
             field_type,
             awkward.types.NumpyType
```

### Comparing `vector-1.0.0/src/vector/backends/numpy.py` & `vector-1.1.0/src/vector/backends/numpy.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     AzimuthalXY,
     Longitudinal,
     LongitudinalEta,
     LongitudinalTheta,
     LongitudinalZ,
     Lorentz,
     LorentzMomentum,
+    Momentum,
     Planar,
     PlanarMomentum,
     Spatial,
     SpatialMomentum,
     Temporal,
     TemporalT,
     TemporalTau,
@@ -48,18 +49,73 @@
     _coordinate_class_to_names,
     _coordinate_order,
     _handler_of,
     _ltype,
     _repr_momentum_to_generic,
     _ttype,
 )
-from vector._typeutils import FloatArray, ScalarCollection
+from vector._typeutils import BoolCollection, FloatArray, ScalarCollection
 
 ArrayLike = ScalarCollection
 
+T = typing.TypeVar("T", bound="VectorNumpy")
+V = typing.TypeVar("V")
+
+SameVectorNumpyType = typing.TypeVar("SameVectorNumpyType", bound="VectorNumpy")
+
+
+def _reduce_sum(
+    a: T,
+    axis: int | None = None,
+    dtype: typing.Any = None,
+    out: typing.Any = None,
+    keepdims: bool | None = None,
+    initial: typing.Any = None,
+    where: typing.Any = None,
+) -> T:
+    if where is not None:
+        raise ValueError("cannot invoke reducer with `where` argument")
+    if initial is not None:
+        raise ValueError("cannot invoke reducer with `initial` argument")
+    if out is not None:
+        raise ValueError("cannot invoke reducer with `out` argument")
+    if dtype is not None:
+        raise ValueError("cannot invoke reducer with `dtype` argument")
+
+    fields: dict[str, typing.Any] = {}
+    if isinstance(a, Lorentz):
+        fields["E"] = numpy.sum(a.t, axis=axis, keepdims=keepdims)
+    if isinstance(a, Spatial):
+        fields["pz"] = numpy.sum(a.z, axis=axis, keepdims=keepdims)
+
+    assert isinstance(a, Planar)
+    fields["px"] = numpy.sum(a.x, axis=axis, keepdims=keepdims)
+    fields["py"] = numpy.sum(a.y, axis=axis, keepdims=keepdims)
+
+    # Convert between representations
+    if not isinstance(a, Momentum):
+        fields = {_repr_momentum_to_generic[n]: v for n, v in fields.items()}
+
+    return array(fields)
+
+
+def _reduce_count_nonzero(
+    a: T, axis: int | None = None, *, keepdims: bool = False
+) -> ScalarCollection:
+    if isinstance(a, Planar):
+        is_nonzero = a.rho2 != 0
+    else:
+        raise AssertionError
+    if isinstance(a, Spatial):
+        is_nonzero = numpy.logical_or(is_nonzero, a.z != 0)
+    if isinstance(a, Lorentz):
+        is_nonzero = numpy.logical_or(is_nonzero, a.t2 != 0)
+
+    return numpy.count_nonzero(is_nonzero, axis=axis, keepdims=keepdims)
+
 
 def _array_from_columns(columns: dict[str, ArrayLike]) -> ArrayLike:
     """
     Converts a dictionary (or columns) of coordinates to an array.
 
     Args:
         columns (dict): The dictionary of coordinates
@@ -91,21 +147,21 @@
             thisdtype = (x, numpy.float64)
 
         if hasattr(columns[x], "shape"):
             thisshape = columns[x].shape
         elif isinstance(columns[x], collections.abc.Sized):
             thisshape = (len(columns[x]),)
         else:
-            raise TypeError(f"column {repr(x)} has no length")
+            raise TypeError(f"column {x!r} has no length")
 
         dtype.append(thisdtype)
         if shape is None:
             shape = thisshape
         elif shape != thisshape:
-            raise ValueError(f"column {repr(x)} has a different shape than the others")
+            raise ValueError(f"column {x!r} has a different shape than the others")
 
     assert shape is not None
     array = numpy.empty(shape, dtype)
     for x in names:
         array[x] = columns[x]
     return array
 
@@ -684,18 +740,33 @@
 
     def allclose(
         self,
         other: VectorProtocol,
         rtol: float | FloatArray = 1e-05,
         atol: float | FloatArray = 1e-08,
         equal_nan: bool | FloatArray = False,
-    ) -> FloatArray:
+    ) -> BoolCollection:
         """Like ``np.ndarray.allclose``, but for VectorNumpy."""
         return self.isclose(other, rtol=rtol, atol=atol, equal_nan=equal_nan).all()
 
+    def sum(
+        self: SameVectorNumpyType,
+        axis: int | None = None,
+        dtype: numpy.dtype[typing.Any] | str | None = None,
+        out: ArrayLike = None,
+        keepdims: bool | None = None,
+        initial: typing.Any = None,
+        where: typing.Any = None,
+    ) -> SameVectorNumpyType:
+        return typing.cast(
+            SameVectorNumpyType,
+            # pylint: disable-next=unexpected-keyword-arg
+            numpy.sum(self, axis=axis, dtype=dtype, out=out, keepdims=keepdims, initial=initial, where=where),  # type: ignore[call-overload]
+        )
+
     def __eq__(self, other: typing.Any) -> typing.Any:
         return numpy.equal(self, other)  # type: ignore[call-overload]
 
     def __ne__(self, other: typing.Any) -> typing.Any:
         return numpy.not_equal(self, other)  # type: ignore[call-overload]
 
     def __reduce__(self) -> str | tuple[typing.Any, ...]:
@@ -929,14 +1000,18 @@
         Implements NumPy's function for ``VectorNumpy`` and its subclasses. The current
         implementation includes ``numpy.isclose`` and ``numpy.allclose``.
         """
         if func is numpy.isclose:
             return type(self).isclose(*args, **kwargs)
         elif func is numpy.allclose:
             return type(self).allclose(*args, **kwargs)
+        elif func is numpy.sum:
+            return _reduce_sum(*args, **kwargs)
+        elif func is numpy.count_nonzero:
+            return _reduce_count_nonzero(*args, **kwargs)
         else:
             return NotImplemented
 
 
 class VectorNumpy2D(VectorNumpy, Planar, Vector2D, FloatArray):  # type: ignore[misc]
     """
     Two dimensional vector class for the NumPy backend. This class can be directly
```

### Comparing `vector-1.0.0/src/vector/backends/object.py` & `vector-1.1.0/src/vector/backends/object.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/tests/test_compute_features.py` & `vector-1.1.0/tests/test_compute_features.py`

 * *Files 2% similar despite different names*

```diff
@@ -262,15 +262,15 @@
         assert node[0].kind == "compare_single", "only do single comparisons"
         assert len(node[0]) == 3
         analyze_expression(expr(node[0][0]), context)
         analyze_expression(expr(node[0][1]), context)
         assert node[0][2].kind == "COMPARE_OP"
         assert (
             node[0][2].attr in allowed_comparisons
-        ), f"add {repr(node[0][2].attr)} to allowed_comparisons"
+        ), f"add {node[0][2].attr!r} to allowed_comparisons"
 
     elif node.kind == "call":
         assert len(node) >= 2
 
         assert node[-1].kind.startswith("CALL_METHOD") or node[-1].kind.startswith(
             "CALL_FUNCTION"
         )
@@ -288,50 +288,48 @@
         print(node)
         raise AssertionError("what is this?")
 
 
 def analyze_unary_operator(node, context):
     assert (
         node.kind in allowed_unary_operators
-    ), f"add {repr(node.kind)} to allowed_unary_operators"
+    ), f"add {node.kind!r} to allowed_unary_operators"
 
 
 def analyze_binary_operator(node, context):
     assert (
         node.kind in allowed_binary_operators
-    ), f"add {repr(node.kind)} to allowed_binary_operators"
+    ), f"add {node.kind!r} to allowed_binary_operators"
 
 
 def analyze_callable(node, context):
     if node.kind == "attribute37":
         assert len(node) == 2
         module = expr(node[0])
         assert module.kind in {"LOAD_FAST", "LOAD_GLOBAL"}
         assert node[1].kind == "LOAD_METHOD"
 
         if module.attr == "lib":
             assert (
                 node[1].attr in allowed_lib_functions
-            ), f"add {repr(node[1].attr)} to allowed_lib_functions"
+            ), f"add {node[1].attr!r} to allowed_lib_functions"
 
         else:
             module_name = ".".join(
                 context.closure.get(module.attr).__name__.split(".")[:-1]
             )
             assert module_name in (
                 "vector._compute.planar",
                 "vector._compute.spatial",
                 "vector._compute.lorentz",
             )
 
     elif node.kind in {"LOAD_GLOBAL", "LOAD_DEREF"}:
         function = context.closure.get(node.attr)
-        assert (
-            function is not None
-        ), f"unrecognized function in scope: {repr(node.attr)}"
+        assert function is not None, f"unrecognized function in scope: {node.attr!r}"
         analyze_function(function)
 
     else:
         print(node)
         raise AssertionError("what is this?")
```

### Comparing `vector-1.0.0/tests/test_issues.py` & `vector-1.1.0/tests/test_issues.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/tests/test_methods.py` & `vector-1.1.0/tests/test_methods.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/tests/backends/test_awkward_numba.py` & `vector-1.1.0/tests/backends/test_awkward_numba.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/tests/backends/test_numba_numpy.py` & `vector-1.1.0/tests/backends/test_numba_numpy.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/tests/backends/test_numba_object.py` & `vector-1.1.0/tests/backends/test_numba_object.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/tests/backends/test_object.py` & `vector-1.1.0/tests/backends/test_object.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/tests/backends/test_operators.py` & `vector-1.1.0/tests/backends/test_operators.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/tests/compute/test_add.py` & `vector-1.1.0/tests/compute/test_add.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/tests/compute/test_conversions.py` & `vector-1.1.0/tests/compute/test_conversions.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/tests/compute/test_dot.py` & `vector-1.1.0/tests/compute/test_dot.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/tests/compute/test_equal.py` & `vector-1.1.0/tests/compute/test_equal.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/tests/compute/test_isclose.py` & `vector-1.1.0/tests/compute/test_isclose.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/tests/compute/test_not_equal.py` & `vector-1.1.0/tests/compute/test_not_equal.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/tests/compute/test_scale.py` & `vector-1.1.0/tests/compute/test_scale.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/tests/compute/test_subtract.py` & `vector-1.1.0/tests/compute/test_subtract.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/tests/compute/test_unit.py` & `vector-1.1.0/tests/compute/test_unit.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/tests/compute/lorentz/test_Et.py` & `vector-1.1.0/tests/compute/lorentz/test_Et.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/tests/compute/lorentz/test_Et2.py` & `vector-1.1.0/tests/compute/lorentz/test_Et2.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/tests/compute/lorentz/test_Mt.py` & `vector-1.1.0/tests/compute/lorentz/test_Mt.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/tests/compute/lorentz/test_Mt2.py` & `vector-1.1.0/tests/compute/lorentz/test_Mt2.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/tests/compute/lorentz/test_beta.py` & `vector-1.1.0/tests/compute/lorentz/test_beta.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/tests/compute/lorentz/test_boostX_beta.py` & `vector-1.1.0/tests/compute/lorentz/test_boostX_beta.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/tests/compute/lorentz/test_boostX_gamma.py` & `vector-1.1.0/tests/compute/lorentz/test_boostX_gamma.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/tests/compute/lorentz/test_boostY_beta.py` & `vector-1.1.0/tests/compute/lorentz/test_boostY_beta.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/tests/compute/lorentz/test_boostY_gamma.py` & `vector-1.1.0/tests/compute/lorentz/test_boostY_gamma.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/tests/compute/lorentz/test_boostZ_beta.py` & `vector-1.1.0/tests/compute/lorentz/test_boostZ_beta.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/tests/compute/lorentz/test_boostZ_gamma.py` & `vector-1.1.0/tests/compute/lorentz/test_boostZ_gamma.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/tests/compute/lorentz/test_boost_beta3.py` & `vector-1.1.0/tests/compute/lorentz/test_boost_beta3.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/tests/compute/lorentz/test_boost_p4.py` & `vector-1.1.0/tests/compute/lorentz/test_boost_p4.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/tests/compute/lorentz/test_deltaRapidityPhi.py` & `vector-1.1.0/tests/compute/lorentz/test_deltaRapidityPhi.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/tests/compute/lorentz/test_deltaRapidityPhi2.py` & `vector-1.1.0/tests/compute/lorentz/test_deltaRapidityPhi2.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/tests/compute/lorentz/test_gamma.py` & `vector-1.1.0/tests/compute/lorentz/test_gamma.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/tests/compute/lorentz/test_rapidity.py` & `vector-1.1.0/tests/compute/lorentz/test_rapidity.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/tests/compute/lorentz/test_t.py` & `vector-1.1.0/tests/compute/lorentz/test_t.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/tests/compute/lorentz/test_t2.py` & `vector-1.1.0/tests/compute/lorentz/test_t2.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/tests/compute/lorentz/test_tau.py` & `vector-1.1.0/tests/compute/lorentz/test_tau.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/tests/compute/lorentz/test_tau2.py` & `vector-1.1.0/tests/compute/lorentz/test_tau2.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/tests/compute/lorentz/test_to_beta3.py` & `vector-1.1.0/tests/compute/lorentz/test_to_beta3.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/tests/compute/planar/test_deltaphi.py` & `vector-1.1.0/tests/compute/planar/test_deltaphi.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/tests/compute/planar/test_phi.py` & `vector-1.1.0/tests/compute/planar/test_phi.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/tests/compute/planar/test_rho.py` & `vector-1.1.0/tests/compute/planar/test_rho.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/tests/compute/planar/test_rho2.py` & `vector-1.1.0/tests/compute/planar/test_rho2.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/tests/compute/planar/test_rotateZ.py` & `vector-1.1.0/tests/compute/planar/test_rotateZ.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/tests/compute/planar/test_x.py` & `vector-1.1.0/tests/compute/planar/test_x.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/tests/compute/planar/test_y.py` & `vector-1.1.0/tests/compute/planar/test_y.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/tests/compute/spatial/test_costheta.py` & `vector-1.1.0/tests/compute/spatial/test_costheta.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/tests/compute/spatial/test_cottheta.py` & `vector-1.1.0/tests/compute/spatial/test_cottheta.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/tests/compute/spatial/test_cross.py` & `vector-1.1.0/tests/compute/spatial/test_cross.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/tests/compute/spatial/test_deltaR.py` & `vector-1.1.0/tests/compute/spatial/test_deltaR.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/tests/compute/spatial/test_deltaR2.py` & `vector-1.1.0/tests/compute/spatial/test_deltaR2.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/tests/compute/spatial/test_deltaangle.py` & `vector-1.1.0/tests/compute/spatial/test_deltaangle.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/tests/compute/spatial/test_deltaeta.py` & `vector-1.1.0/tests/compute/spatial/test_deltaeta.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/tests/compute/spatial/test_eta.py` & `vector-1.1.0/tests/compute/spatial/test_eta.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/tests/compute/spatial/test_mag.py` & `vector-1.1.0/tests/compute/spatial/test_mag.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/tests/compute/spatial/test_mag2.py` & `vector-1.1.0/tests/compute/spatial/test_mag2.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/tests/compute/spatial/test_rotateX.py` & `vector-1.1.0/tests/compute/spatial/test_rotateX.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/tests/compute/spatial/test_rotateY.py` & `vector-1.1.0/tests/compute/spatial/test_rotateY.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/tests/compute/spatial/test_rotate_axis.py` & `vector-1.1.0/tests/compute/spatial/test_rotate_axis.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/tests/compute/spatial/test_rotate_euler.py` & `vector-1.1.0/tests/compute/spatial/test_rotate_euler.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/tests/compute/spatial/test_rotate_quaternion.py` & `vector-1.1.0/tests/compute/spatial/test_rotate_quaternion.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/tests/compute/spatial/test_theta.py` & `vector-1.1.0/tests/compute/spatial/test_theta.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/tests/compute/spatial/test_z.py` & `vector-1.1.0/tests/compute/spatial/test_z.py`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/tests/samples/issue-161-v2.pkl` & `vector-1.1.0/tests/samples/issue-161-v2.pkl`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/tests/samples/issue-161.pkl` & `vector-1.1.0/tests/samples/issue-161.pkl`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/.gitignore` & `vector-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/LICENSE` & `vector-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vector-1.0.0/README.md` & `vector-1.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 [![PyPI platforms][pypi-platforms]][pypi-link]
 [![PyPI version][pypi-version]][pypi-link]
 [![Conda latest release][conda-version]][conda-link]
 [![DOI][zenodo-badge]][zenodo-link]
 [![LICENSE][license-badge]][license-link]
 [![Scikit-HEP][sk-badge]][sk-link]
 
-Vector is a Python 3.7+ library for 2D, 3D, and [Lorentz vectors](https://en.wikipedia.org/wiki/Special_relativity#Physics_in_spacetime), especially _arrays of vectors_, to solve common physics problems in a NumPy-like way.
+Vector is a Python 3.8+ library (Python 3.6 and 3.7 supported till `v0.9.0` and `v1.0.0`, respectively) for 2D, 3D, and [Lorentz vectors](https://en.wikipedia.org/wiki/Special_relativity#Physics_in_spacetime), especially _arrays of vectors_, to solve common physics problems in a NumPy-like way.
 
 Main features of Vector:
 
 - Pure Python with NumPy as its only dependency. This makes it easier to install.
 - Vectors may be represented in a variety of coordinate systems: Cartesian, cylindrical, pseudorapidity, and any combination of these with time or proper time for Lorentz vectors. In all, there are 12 coordinate systems: {_x_-_y_ vs _ρ_-_φ_ in the azimuthal plane} × {_z_ vs _θ_ vs _η_ longitudinally} × {_t_ vs _τ_ temporally}.
 - Uses names and conventions set by [ROOT](https://root.cern/)'s [TLorentzVector](https://root.cern.ch/doc/master/classTLorentzVector.html) and [Math::LorentzVector](https://root.cern.ch/doc/master/classROOT_1_1Math_1_1LorentzVector.html), as well as [scikit-hep/math](https://github.com/scikit-hep/scikit-hep/tree/master/skhep/math), [uproot-methods TLorentzVector](https://github.com/scikit-hep/uproot3-methods/blob/master/uproot3_methods/classes/TLorentzVector.py), [henryiii/hepvector](https://github.com/henryiii/hepvector), and [coffea.nanoevents.methods.vector](https://coffeateam.github.io/coffea/modules/coffea.nanoevents.methods.vector.html).
 - Implemented on a variety of backends:
```

### Comparing `vector-1.0.0/pyproject.toml` & `vector-1.1.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -11,51 +11,47 @@
 readme = { file = "README.md", content-type = "text/markdown" }
 keywords = [
   "vector",
 ]
 license = "BSD-3-Clause"
 maintainers = [ {name = "The Scikit-HEP admins", email = "scikit-hep-admins@googlegroups.com"} ]
 authors = [ {name = "Jim Pivarski, Henry Schreiner, Eduardo Rodrigues", email = "eduardo.rodrigues@cern.ch"} ]
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 classifiers = [
-    "Development Status :: 5 - Production/Stable",
-    "Intended Audience :: Developers",
-    "Intended Audience :: Science/Research",
-    "License :: OSI Approved :: BSD License",
-    "Operating System :: OS Independent",
-    "Programming Language :: Python",
-    "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.7",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
-    "Topic :: Scientific/Engineering",
-    "Topic :: Scientific/Engineering :: Information Analysis",
-    "Topic :: Scientific/Engineering :: Mathematics",
-    "Topic :: Scientific/Engineering :: Physics",
-    "Typing :: Typed",
+  "Development Status :: 5 - Production/Stable",
+  "Intended Audience :: Developers",
+  "Intended Audience :: Science/Research",
+  "License :: OSI Approved :: BSD License",
+  "Operating System :: OS Independent",
+  "Programming Language :: Python",
+  "Programming Language :: Python :: 3 :: Only",
+  "Programming Language :: Python :: 3.8",
+  "Programming Language :: Python :: 3.9",
+  "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
+  "Topic :: Scientific/Engineering",
+  "Topic :: Scientific/Engineering :: Information Analysis",
+  "Topic :: Scientific/Engineering :: Mathematics",
+  "Topic :: Scientific/Engineering :: Physics",
+  "Typing :: Typed",
 ]
 dynamic = [
   "version",
 ]
 dependencies = [
-  'importlib-metadata>=0.22; python_version < "3.8"',
   "numpy>=1.13.3",
   "packaging>=19",
-  'typing-extensions; python_version < "3.8"',
 ]
 [project.optional-dependencies]
 awkward = [
   "awkward>=1.2",
 ]
 dev = [
   "awkward>=1.2",
-  'numba>=0.50; python_version < "3.11"',
+  "numba>=0.57",
   "papermill>=2.4",
   "pytest>=6",
   "pytest-cov>=3",
   "xdoctest>=1",
 ]
 docs = [
   "awkward>=1.2",
@@ -73,31 +69,64 @@
   "pytest-cov>=3",
   "xdoctest>=1",
 ]
 test-extras = [
   "spark-parser",
   "uncompyle6",
 ]
-
 [project.urls]
 "Bug Tracker" = "https://github.com/scikit-hep/vector/issues"
 Changelog = "https://vector.readthedocs.io/en/latest/changelog.html"
 Discussions = "https://github.com/scikit-hep/vector/discussions"
 Documentation = "https://vector.readthedocs.io/"
 Homepage = "https://github.com/scikit-hep/vector"
-
 [project.entry-points.numba_extensions]
 init = "vector:register_numba"
 
-
-
 [tool.hatch]
 version.source = "vcs"
 build.hooks.vcs.version-file = "src/vector/version.py"
 
+[tool.ruff]
+select = [
+  "E", "F", "W", # flake8
+  "B", "B904",   # flake8-bugbear
+  "I",           # isort
+  "C4",          # flake8-comprehensions
+  "ISC",         # flake8-implicit-str-concat
+  "PGH",         # pygrep-hooks
+  "PIE",         # flake8-pie
+  "PL",          # pylint
+  "PT",          # flake8-pytest-style
+  "RUF",         # Ruff-specific
+  "SIM",         # flake8-simplify
+  "T20",         # flake8-print
+  "UP",          # pyupgrade
+  "YTT",         # flake8-2020
+]
+extend-ignore = [
+  "PLR",   # Design related pylint codes
+  "E501",  # Line too long
+]
+target-version = "py38"
+typing-modules = ["vector._typeutils"]
+src = ["src"]
+unfixable = [
+  "T20",  # Removes print statements
+  "F841", # Removes unused variables
+]
+exclude = []
+isort.required-imports = ["from __future__ import annotations"]
+
+[tool.ruff.per-file-ignores]
+"noxfile.py" = ["T20"]
+"tests/*" = ["T20"]
+"src/vector/backends/_numba_object.py" = ["PGH003"]
+"tests/backends/test_operators.py" = ["SIM201", "SIM202"]
+
 [tool.pytest.ini_options]
 minversion = "6.0"
 xfail_strict = true
 addopts = [
     "-ra",
     "--strict-markers",
     "--strict-config",
@@ -138,18 +167,16 @@
   "numba.*",
   "awkward.*",
 ]
 ignore_missing_imports = true
 disallow_untyped_defs = false
 disallow_untyped_calls = false
 
-
-
 [tool.pylint]
-master.py-version = "3.7"
+master.py-version = "3.8"
 reports.output-format = "colorized"
 similarities.ignore-imports = "yes"
 master.jobs = "0"
 messages_control.enable = [
   "useless-suppression",
 ]
 messages_control.disable = [
@@ -198,44 +225,7 @@
   "pointless-string-statement",
   "useless-option-value",
   "cast_python_value",
   "unknown-option-value",
   "no-else-raise",
   "unidiomatic-typecheck",
 ]
-
-[tool.ruff]
-select = [
-  "E", "F", "W", # flake8
-  "B", "B904",   # flake8-bugbear
-  "I",           # isort
-  "C4",          # flake8-comprehensions
-  "ISC",         # flake8-implicit-str-concat
-  "PGH",         # pygrep-hooks
-  "PIE",         # flake8-pie
-  "PL",          # pylint
-  "PT",          # flake8-pytest-style
-  "RUF",         # Ruff-specific
-  "SIM",         # flake8-simplify
-  "T20",         # flake8-print
-  "UP",          # pyupgrade
-  "YTT",         # flake8-2020
-]
-extend-ignore = [
-  "PLR",   # Design related pylint codes
-  "E501",  # Line too long
-]
-target-version = "py37"
-typing-modules = ["vector._typeutils"]
-src = ["src"]
-unfixable = [
-  "T20",  # Removes print statements
-  "F841", # Removes unused variables
-]
-exclude = []
-isort.required-imports = ["from __future__ import annotations"]
-
-[tool.ruff.per-file-ignores]
-"noxfile.py" = ["T20"]
-"tests/*" = ["T20"]
-"src/vector/backends/_numba_object.py" = ["PGH003"]
-"tests/backends/test_operators.py" = ["SIM201", "SIM202"]
```

### Comparing `vector-1.0.0/PKG-INFO` & `vector-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector
-Version: 1.0.0
+Version: 1.1.0
 Summary: Vector classes and utilities
 Project-URL: Bug Tracker, https://github.com/scikit-hep/vector/issues
 Project-URL: Changelog, https://vector.readthedocs.io/en/latest/changelog.html
 Project-URL: Discussions, https://github.com/scikit-hep/vector/discussions
 Project-URL: Documentation, https://vector.readthedocs.io/
 Project-URL: Homepage, https://github.com/scikit-hep/vector
 Author-email: "Jim Pivarski, Henry Schreiner, Eduardo Rodrigues" <eduardo.rodrigues@cern.ch>
@@ -14,36 +14,32 @@
 Keywords: vector
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Typing :: Typed
-Requires-Python: >=3.7
-Requires-Dist: importlib-metadata>=0.22; python_version < '3.8'
+Requires-Python: >=3.8
 Requires-Dist: numpy>=1.13.3
 Requires-Dist: packaging>=19
-Requires-Dist: typing-extensions; python_version < '3.8'
 Provides-Extra: awkward
 Requires-Dist: awkward>=1.2; extra == 'awkward'
 Provides-Extra: dev
 Requires-Dist: awkward>=1.2; extra == 'dev'
-Requires-Dist: numba>=0.50; python_version < '3.11' and extra == 'dev'
+Requires-Dist: numba>=0.57; extra == 'dev'
 Requires-Dist: papermill>=2.4; extra == 'dev'
 Requires-Dist: pytest-cov>=3; extra == 'dev'
 Requires-Dist: pytest>=6; extra == 'dev'
 Requires-Dist: xdoctest>=1; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: awkward>=1.2; extra == 'docs'
 Requires-Dist: ipykernel; extra == 'docs'
@@ -78,15 +74,15 @@
 [![PyPI platforms][pypi-platforms]][pypi-link]
 [![PyPI version][pypi-version]][pypi-link]
 [![Conda latest release][conda-version]][conda-link]
 [![DOI][zenodo-badge]][zenodo-link]
 [![LICENSE][license-badge]][license-link]
 [![Scikit-HEP][sk-badge]][sk-link]
 
-Vector is a Python 3.7+ library for 2D, 3D, and [Lorentz vectors](https://en.wikipedia.org/wiki/Special_relativity#Physics_in_spacetime), especially _arrays of vectors_, to solve common physics problems in a NumPy-like way.
+Vector is a Python 3.8+ library (Python 3.6 and 3.7 supported till `v0.9.0` and `v1.0.0`, respectively) for 2D, 3D, and [Lorentz vectors](https://en.wikipedia.org/wiki/Special_relativity#Physics_in_spacetime), especially _arrays of vectors_, to solve common physics problems in a NumPy-like way.
 
 Main features of Vector:
 
 - Pure Python with NumPy as its only dependency. This makes it easier to install.
 - Vectors may be represented in a variety of coordinate systems: Cartesian, cylindrical, pseudorapidity, and any combination of these with time or proper time for Lorentz vectors. In all, there are 12 coordinate systems: {_x_-_y_ vs _ρ_-_φ_ in the azimuthal plane} × {_z_ vs _θ_ vs _η_ longitudinally} × {_t_ vs _τ_ temporally}.
 - Uses names and conventions set by [ROOT](https://root.cern/)'s [TLorentzVector](https://root.cern.ch/doc/master/classTLorentzVector.html) and [Math::LorentzVector](https://root.cern.ch/doc/master/classROOT_1_1Math_1_1LorentzVector.html), as well as [scikit-hep/math](https://github.com/scikit-hep/scikit-hep/tree/master/skhep/math), [uproot-methods TLorentzVector](https://github.com/scikit-hep/uproot3-methods/blob/master/uproot3_methods/classes/TLorentzVector.py), [henryiii/hepvector](https://github.com/henryiii/hepvector), and [coffea.nanoevents.methods.vector](https://coffeateam.github.io/coffea/modules/coffea.nanoevents.methods.vector.html).
 - Implemented on a variety of backends:
```

