# Created by: vanilla
# $FreeBSD$

PORTREVISION=	1
CATEGORIES=	chinese

MAINTAINER=	vanilla@FreeBSD.org
COMMENT=	zh-tw cursor movement friendly, wrapping clean irssi

CONFLICTS?=	irssi-*
MASTERDIR=	${.CURDIR}/../../irc/irssi

EXTRA_PATCHES=	${.CURDIR}/files/patch-irssi.conf \
		${.CURDIR}/files/patch-utf8_break

.include "${MASTERDIR}/Makefile"
