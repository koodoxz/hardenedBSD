# $FreeBSD$

# Vendor sources and generated files
LDNSDIR= ${SRCTOP}/contrib/ldns
UNBOUNDDIR= ${SRCTOP}/contrib/unbound

.PATH: ${UNBOUNDDIR} ${UNBOUNDDIR}/daemon ${UNBOUNDDIR}/util ${UNBOUNDDIR}/doc

PROG=	unbound
SRCS=	acl_list.c cachedump.c daemon.c remote.c stats.c ub_event.c \
	unbound.c worker.c
CFLAGS+=	-I${UNBOUNDDIR} -I${LDNSDIR}
LIBADD=	unbound util ssl crypto pthread
MAN=	unbound.8 unbound.conf.5
NOCFI=	yes

.include <bsd.prog.mk>
