# Created by: Franco Fichtner <franco@opnsense.org>
# $FreeBSD$

PORTNAME=	opnsense-update
PORTVERSION=	18.7.1
PORTREVISION=	0 # GH_TAGNAME
CATEGORIES=	sysutils

MAINTAINER=	franco@opnsense.org
COMMENT=	OPNsense update utilities

LICENSE=	BSD2CLAUSE

LIB_DEPENDS+=	libucl.so:textproc/libucl

USES=		ssl

USE_HARDENING=	safestack

USE_GITHUB=	yes
GH_ACCOUNT=	opnsense
GH_PROJECT=	update
#GH_TAGNAME=	979fcfc

.include <bsd.port.mk>
