# Created by: Wen Heping <wenheping@gmail.com>
# $FreeBSD$

PORTNAME=	mcve
PORTVERSION=	7.0.3
PORTREVISION=	2
CATEGORIES=	devel pear
MASTER_SITES=	http://pecl.php.net/get/
PKGNAMEPREFIX=	pecl-
DIST_SUBDIR=	PECL

MAINTAINER=	ports@FreeBSD.org
COMMENT=	PECL Extension for Interface the MCVE/Monetra API

DEPRECATED=	Works only with EOL php 5.5
EXPIRATION_DATE=	2016-10-20

LICENSE=	PHP30

LIB_DEPENDS=	libmonetra.so:devel/libmonetra

USES=		php:ext tar:tgz
USE_OPENSSL=	yes
IGNORE_WITH_PHP=	56 70
CONFIGURE_ARGS+=	--with-mcve="${LOCALBASE}"

post-patch:
	${REINPLACE_CMD} -e '/SEARCH_PATH/ s,=",="${LOCALBASE} ${PREFIX} ,' \
		${WRKSRC}/config.m4

.include <bsd.port.mk>
