# $OpenBSD: Makefile.template,v 1.73 2016/01/11 09:17:22 sthen Exp $

COMMENT =	a key value storage for Lua optimised for i18n

V =		1.3-1
DISTNAME =	lua-say-${V}
PKGNAME =	lua-say-${V:S/-/./g}

GH_ACCOUNT =	olivine-labs
GH_PROJECT =	say
GH_TAGNAME =	v${V}

CATEGORIES =	devel

MAINTAINER =		Florian Stinglmayr <florian@n0la.org>

#MIT
PERMIT_PACKAGE_CDROM =	Yes

FLAVORS =	lua52 lua53
FLAVOR ?=

MODULES =		lang/lua

NO_BUILD =		Yes
NO_TEST =		Yes

do-install:
	${INSTALL_DATA_DIR} ${MODLUA_DATADIR} ${MODLUA_DATADIR}/say
	${INSTALL_DATA} ${WRKSRC}/src/init.lua ${MODLUA_DATADIR}/say

.include <bsd.port.mk>
