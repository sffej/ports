# Original from: John Walker http://www.fourmilab.ch/random/

CATEGORIES=		misc
COMMENT=		pseudo random number sequence test program

DISTNAME=		ent-1.0
DISTFILES=		${DISTNAME}{random}.zip
REVISION=		1
EXTRACT_SUFX=		.zip

HOMEPAGE=		https://www.fourmilab.ch/random/
SITES=			https://www.fourmilab.ch/random/

WRKDIST=		${WRKDIR}
ALL_TARGET=		ent

MAKE_FLAGS=		CFLAGS="${CFLAGS}" CC="${CC}"

# Public Domain; see ent.html
PERMIT_PACKAGE=	Yes

WANTLIB += c m

NO_TEST=		Yes

do-install:
	${INSTALL_PROGRAM} ${WRKSRC}/ent ${PREFIX}/bin
	${INSTALL_MAN} ${FILESDIR}/ent.1 ${PREFIX}/man/man1

.include <bsd.port.mk>
