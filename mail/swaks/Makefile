COMMENT=	swiss army knife SMTP transaction tester

DISTNAME=	swaks-20240103.0

CATEGORIES=	mail

HOMEPAGE=	https://jetmore.org/john/code/swaks/
SITES=		${HOMEPAGE}

MAINTAINER=	Jeremie Courreges-Anglas <jca@wxcvbn.org>

# GPLv2+
PERMIT_PACKAGE=	Yes

RUN_DEPENDS=	net/p5-Net-DNS \
		security/p5-Net-SSLeay \
		security/p5-Authen-SASL \
		security/p5-Authen-NTLM

NO_TEST=	Yes

PKG_ARCH=	*

do-build:
	cd ${WRKSRC} && pod2man swaks swaks.1

do-install:
	${INSTALL_SCRIPT} ${WRKSRC}/swaks ${PREFIX}/bin/swaks
	${INSTALL_MAN} ${WRKSRC}/swaks.1 ${PREFIX}/man/man1
	${INSTALL_DATA_DIR} ${PREFIX}/share/doc/swak
	${INSTALL_DATA} ${WRKSRC}/doc/{recipes,ref}.txt \
	    ${PREFIX}/share/doc/swak

.include <bsd.port.mk>
