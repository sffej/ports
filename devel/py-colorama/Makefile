# !!! do not update blindly: sysutils/awscli requires a specific version

COMMENT=		print colored terminal text from Python apps

MODPY_EGG_VERSION=	0.4.6
DISTNAME=		colorama-${MODPY_EGG_VERSION}
PKGNAME=		py-${DISTNAME}

CATEGORIES=		devel

HOMEPAGE=		https://github.com/tartley/colorama

MAINTAINER=		Antoine Jacoutot <ajacoutot@openbsd.org>

# BSD
PERMIT_PACKAGE=	Yes

MODULES=		lang/python

MODPY_PI=		Yes
MODPY_PYBUILD=		hatchling

FLAVORS=		python3
FLAVOR=			python3

.include <bsd.port.mk>
