# SPDX-License-Identifier: BSD-3-Clause
# SPDX-FileCopyrightText: 2023 Rachel Mant <git@dragonmux.network>
commonSrcs = [
	'crc32.c',
	'fastmath.c',
	'huffman-bcl.c',
	'tags.c',
]

common = static_library(
	'common',
	commonSrcs,
	include_directories: includes,
	gnu_symbol_visibility: 'inlineshidden',
	install: true
)
