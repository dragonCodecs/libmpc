# SPDX-License-Identifier: BSD-3-Clause
# SPDX-FileCopyrightText: 2023 Rachel Mant <git@dragonmux.network>
libmpcencSrcs = [
	'analy_filter.c',
	'bitstream.c',
	'encode_sv7.c',
	'huffsv7.c',
	'quant.c',
]
libmpcencInc = include_directories('.')

libmpcenc = static_library(
	'libmpcenc',
	libmpcencSrcs,
	include_directories: includes,
	link_with: [common],
	dependencies: [maths],
	gnu_symbol_visibility: 'inlineshidden',
	install: true
)
