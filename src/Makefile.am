# Copyright (C) (2007) (Benoit Favre) <favre@icsi.berkeley.edu>
#
# This program is free software; you can redistribute it and/or 
# modify it under the terms of the GNU Lesser General Public License 
# as published by the Free Software Foundation; either 
# version 2 of the License, or (at your option) any later 
# version.
#
# This program is distributed in the hope that it will be useful,
# but WITHOUT ANY WARRANTY; without even the implied warranty of
# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
# GNU Lesser General Public License for more details.
#
# You should have received a copy of the GNU Lesser General Public License
# along with this program; if not, write to the Free Software
# Foundation, Inc., 675 Mass Ave, Cambridge, MA 02139, USA.

#MAKEFLAGS=-s

# should move to -Werror (all warnings are errors)
INCLUDES=-Wall -Werror-implicit-function-declaration -L/opt/local/lib

utils = utils/vector.c utils/string.c utils/hashtable.c utils/array.c utils/mapped.c utils/threads.c utils/debug.c utils/file.c utils/common.c
utils += utils/vector.h utils/string.h utils/hashtable.h utils/array.h utils/mapped.h utils/threads.h utils/debug.h utils/file.h utils/common.h

bin_PROGRAMS = icsiboost
check_PROGRAMS = utils_test test_api
icsiboost_SOURCES = icsiboost.c $(utils)
test_api_SOURCES = test_api.cc IcsiBoost.cc
#icsiboost_LDADD  = -lm -lpthread -lz -lpcre
#perceptron_SOURCES = perceptron.c $(utils) $(classifier)
#perceptron_LDADD  = -lm -lpthread -lz -lpcre
utils_test_SOURCES = utils_test.c $(utils)
#utils_test_LDADD  = -lm -lz -lpcre

EXTRA_DIST = test_uci.sh
