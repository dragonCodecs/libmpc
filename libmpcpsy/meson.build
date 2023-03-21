# SPDX-License-Identifier: BSD-3-Clause
# SPDX-FileCopyrightText: 2023 Rachel Mant <git@dragonmux.network>
libmpcpsySrcs = [
	'ans.c',
	'cvd.c',
	'fft4g.c',
	'fft_routines.c',
	'profile.c',
	'psy.c',
	'psy_tab.c',
]
libmpcpsyInc = include_directories('.')

libmpcpsy = static_library(
	'libmpcpsy',
	libmpcpsySrcs,
	include_directories: includes,
	link_with: [common],
	dependencies: [maths],
	gnu_symbol_visibility: 'inlineshidden',
	install: true
)
