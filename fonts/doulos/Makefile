COMMENT =		Unicode-based font for Roman and Cyrillic

MODFONT_FAMILY =	doulos
MODFONT_VERSION =	6.101
DISTNAME =		DoulosSIL-${MODFONT_VERSION}
CATEGORIES =		fonts

HOMEPAGE =		https://software.sil.org/doulos/

MAINTAINER =		George Rosamond <george@nycbug.org>

# SIL OFL 1.1
PERMIT_PACKAGE =	Yes

SITES =			https://software.sil.org/downloads/r/doulos/

MODULES =		font

NO_BUILD =		Yes
NO_TEST =		Yes

WRKDIST =		${WRKDIR}/${DISTNAME}
DOCDIR =		${PREFIX}/share/doc/doulos

post-install:
	${INSTALL_DATA_DIR} ${DOCDIR}
	${INSTALL_DATA} ${WRKDIST}/*.txt ${DOCDIR}

.include <bsd.port.mk>
