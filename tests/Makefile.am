# Written by Simon Josefsson <simon@josefsson.org>.
# Copyright (c) 2011-2012 Yubico AB
# All rights reserved.
#
# Redistribution and use in source and binary forms, with or without
# modification, are permitted provided that the following conditions are
# met:
#
#   * Redistributions of source code must retain the above copyright
#      notice, this list of conditions and the following disclaimer.
#
#   * Redistributions in binary form must reproduce the above
#      copyright notice, this list of conditions and the following
#      disclaimer in the documentation and/or other materials provided
#      with the distribution.
#
# THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
# "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT
# LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR
# A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT
# OWNER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL,
# SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT
# LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
# DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY
# THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
# (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
# OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.

# Self tests.

AM_CPPFLAGS = @LIBCURL_CPPFLAGS@
AM_LDFLAGS = -no-install
AM_CFLAGS=-I$(srcdir)/..
LDADD = ../libykclient.la -lcurl
selftest_SOURCES = selftest.c ../b64/cencode.c ../b64/cdecode.c \
                   ../rfc4634/hmac.c ../rfc4634/sha1.c ../rfc4634/usha.c  \
                   ../rfc4634/sha224-256.c ../rfc4634/sha384-512.c

check_PROGRAMS = selftest
TESTS = $(check_PROGRAMS)
