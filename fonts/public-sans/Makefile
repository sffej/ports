COMMENT =		strong, neutral, principles-driven typeface

V =			2.001
DISTNAME =		public-sans-v$V
PKGNAME =		public-sans-$V

CATEGORIES =		fonts

HOMEPAGE =		https://public-sans.digital.gov/

# SIL OFL 1.1
PERMIT_PACKAGE =	Yes

SITES =		https://github.com/uswds/public-sans/releases/download/v$V/

EXTRACT_SUFX =		.zip

NO_BUILD =		Yes
NO_TEST =		Yes

WRKDIST =		${WRKDIR}

PKG_ARCH =		*

FONTDIR =		${PREFIX}/share/fonts/public-sans

FIX_EXTRACT_PERMISSIONS =	Yes

do-install:
	${INSTALL_DATA_DIR} ${FONTDIR}
	${INSTALL_DATA} ${WRKDIST}/fonts/*/*.{ttf,otf} \
		${FONTDIR}

.include <bsd.port.mk>
