COMMENT=	AJAX framework for perl

MODULES=	cpan
PKG_ARCH=	*
CATEGORIES=	www
SITES=		${SITE_PERL_CPAN:=HTML/}
SITES.js=	http://script.aculo.us/dist/
DISTNAME=	HTML-Prototype-1.48

DISTFILES.js= 	scriptaculous-js-1.7.0.tar.gz

HOMEPAGE=	http://prototype.conio.net/

post-extract:
	PROTODIR=${WRKDIST} ACULOUSDIR=${WRKDIR}/scriptaculous-js-1.7.0 perl ${FILESDIR}/update Controls src/controls DragDrop src/dragdrop Effects src/effects Js lib/prototype

# Perl licence, javascript code is MIT like
PERMIT_PACKAGE=	Yes

FIX_CRLF_FILES=	lib/HTML/Prototype.pm

CONFIGURE_STYLE=	modbuild

BUILD_DEPENDS=	${RUN_DEPENDS}
RUN_DEPENDS=	www/p5-HTML-Tree devel/p5-Class-Accessor

MAKE_ENV+=	TEST_POD=Yes

.include <bsd.port.mk>
