# Note that the languages C,C++, Python3, Java, Haskel and Pascal are installed in the main image
ARG VERSION=7.3.2
FROM domjudge/judgehost:${VERSION}
ENV LANG_KOTLIN=yes
# Only used for company teams
ENV LANG_CSHARP=no
# Python 2 is no longer an ICPC language
ENV LANG_PY2=no
ENV LANG_PYPY3=no
ENV CHROOT=/chroot/domjudge
COPY install_languages.sh /
ARG KOTLIN_VERSION=1.4.32
COPY --chown=domjudge:domjudge kotlinc /usr/local/lib/kotlinc

