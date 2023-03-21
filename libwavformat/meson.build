# SPDX-License-Identifier: BSD-3-Clause
# SPDX-FileCopyrightText: 2023 Rachel Mant <git@dragonmux.network>
libwavformatSrcs = [
	'input.c',
	'output.c',
]
libwavformatInc = include_directories('.')

libwavformat = static_library(
	'libwavformat',
	libwavformatSrcs,
	include_directories: includes,
	link_with: [common],
	dependencies: [maths],
	gnu_symbol_visibility: 'inlineshidden',
	name_prefix: '',
	install: true
)
