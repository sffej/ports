COMMENT=	PostIt (R) messages onto your X11 screen

DISTNAME=	xpostit3.3.1
PKGNAME=	xpostit-3.3.1
REVISION=	3
CATEGORIES=	x11

SITES=		${SITE_R5CONTRIB}
EXTRACT_SUFX=	.tar.Z

# BSD
PERMIT_PACKAGE=	Yes

WANTLIB=	ICE SM X11 Xau Xaw Xdmcp Xext Xmu Xpm Xt c

CONFIGURE_STYLE=	imake
WRKDIST=	${WRKDIR}/xpostit

NO_TEST=	Yes

.include <bsd.port.mk>
