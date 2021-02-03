# $FreeBSD$

PORTNAME=	sphinx-rtd-theme
DISTVERSION=	0.5.1
CATEGORIES=	textproc python
MASTER_SITES=	CHEESESHOP
PKGNAMEPREFIX=	${PYTHON_PKGNAMEPREFIX}
DISTNAME=	${PORTNAME:S/-/_/g}-${DISTVERSIONPREFIX}${DISTVERSION}${DISTVERSIONSUFFIX}

MAINTAINER=	y@trombik.org
COMMENT=	Read the Docs theme for Sphinx

LICENSE=	MIT
LICENSE_FILE=	${WRKSRC}/LICENSE

USES=		python
USE_PYTHON=	autoplist distutils
BUILD_DEPENDS=	\
	${PYTHON_PKGNAMEPREFIX}sphinx>0:textproc/py-sphinx@${PY_FLAVOR}
NO_ARCH=	yes

# XXX setup.py include a logic to rebuild the sources with webpack. disable
# it.
MAKE_ENV=	CI=y

.include <bsd.port.mk>
