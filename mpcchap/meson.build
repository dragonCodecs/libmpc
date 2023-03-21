# SPDX-License-Identifier: BSD-3-Clause
# SPDX-FileCopyrightText: 2023 Rachel Mant <git@dragonmux.network>
mpcchapSrcs = [
	'mpcchap.c',
	'dictionary.c',
	'iniparser.c',
]

mpcchap = executable(
	'mpcchap',
	mpcchapSrcs,
	include_directories: includes,
	link_with: [common, libmpcdec, libmpcenc],
	dependencies: [maths, libcuefile],
	gnu_symbol_visibility: 'inlineshidden',
	install: true
)
