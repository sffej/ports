COMMENT =	geospatial raster data API and CLI

MODPY_EGG_VERSION =	1.3.2
DISTNAME =	rasterio-${MODPY_EGG_VERSION}
PKGNAME =	py-${DISTNAME}
REVISION =	2

CATEGORIES =	geo

HOMEPAGE =	https://rasterio.readthedocs.io/en/latest/

MAINTAINER = 	Martin Reindl <martin@catai.org>

# BSD
PERMIT_PACKAGE =	Yes

MODULES =	lang/python

FLAVORS =	python3
FLAVOR =	python3

COMPILER =	base-clang ports-gcc

MODPY_PYBUILD =	setuptools
MODPY_PI =	Yes

LIB_DEPENDS =	geo/gdal
WANTLIB +=	${COMPILER_LIBCXX} gdal m

BUILD_DEPENDS +=	lang/cython${MODPY_FLAVOR} \
			math/py-numpy${MODPY_FLAVOR} \
			math/py-oldest-supported-numpy${MODPY_FLAVOR}

RUN_DEPENDS =	geo/py-cligj${MODPY_FLAVOR}>=0.5 \
		net/py-boto3${MODPY_FLAVOR} \
		devel/py-attrs${MODPY_FLAVOR} \
		devel/py-click${MODPY_FLAVOR} \
		devel/py-click-plugins${MODPY_FLAVOR} \
		math/py-numpy${MODPY_FLAVOR} \
		math/py-snuggs${MODPY_FLAVOR} \
		math/py-affine${MODPY_FLAVOR}

# test_read_no_band requires hdf5 support in GDAL
# requires datafiles only on github...
NO_TEST =	Yes
TEST_DEPENDS =	devel/py-certifi${MODPY_FLAVOR} \
		devel/py-hypothesis${MODPY_FLAVOR} \
		devel/py-mock${MODPY_FLAVOR} \
		devel/py-test${MODPY_FLAVOR} \
		devel/py-test-cov${MODPY_FLAVOR} \
		geo/py-shapely${MODPY_FLAVOR}

.include <bsd.port.mk>
