# Created by: Edwin Groothuis <edwin@mavetju.org>
# $FreeBSD$

PORTNAME=	e169-stats
PORTVERSION=	0.6
PORTREVISION=	1
CATEGORIES=	net
MASTER_SITES=	http://www.mavetju.org/download/

MAINTAINER=	ports@FreeBSD.org
COMMENT=	Curses realtime statistics for the Huawei E169 modem

LICENSE=	NONE

DEPRECATED=	unknown license
EXPIRATION_DATE=	2018-08-15

USES=		ncurses
PLIST_FILES=	bin/e169-stats

do-build:
	${CC} ${CFLAGS} -o ${WRKSRC}/e169-stats ${WRKSRC}/e169-stats.c \
		${LDFLAGS} -lncurses

do-install:
	${INSTALL_PROGRAM} ${WRKSRC}/e169-stats ${STAGEDIR}${PREFIX}/bin

.include <bsd.port.mk>
