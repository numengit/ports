# Created by: Emanuel Haupt <ehaupt@critical.ch>
# $FreeBSD$

PORTNAME=	xymms
DISTVERSION=	0.9.1
PORTREVISION=	7
CATEGORIES=	audio
MASTER_SITES=	SF
PKGNAMEPREFIX=	xmms-

MAINTAINER=	ehaupt@FreeBSD.org
COMMENT=	Sega Genesis GYM plugin for XMMS

LIB_DEPENDS=	libxmms.so:multimedia/xmms

GNU_CONFIGURE=	yes
USES=		gettext-runtime libtool
USE_GNOME=	gtk12
USE_XORG=	x11 xext xi
USE_LDCONFIG=	yes
CONFIGURE_ARGS=	--disable-static

PLIST_FILES=	lib/xmms/Input/libxymms.so \
		%%EXAMPLESDIR%%/sample.gym

post-install:
	@${MKDIR} ${STAGEDIR}${EXAMPLESDIR}
	${INSTALL_DATA} ${WRKSRC}/samples/sample.gym ${STAGEDIR}${EXAMPLESDIR}
	${STRIP_CMD} ${STAGEDIR}${PREFIX}/lib/xmms/Input/libxymms.so

.include <bsd.port.mk>
