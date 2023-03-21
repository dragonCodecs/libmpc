# SPDX-License-Identifier: BSD-3-Clause
# SPDX-FileCopyrightText: 2023 Rachel Mant <git@dragonmux.network>
libmpcdecSrcs = [
	'huffman.c',
	'mpc_decoder.c',
	'mpc_reader.c',
	'streaminfo.c',
	'mpc_bits_reader.c',
	'mpc_demux.c',
	'requant.c',
	'synth_filter.c',
]

libmpcdec = library(
	'libmpcdec',
	libmpcdecSrcs,
	include_directories: includes,
	link_with: [common],
	dependencies: [maths],
	gnu_symbol_visibility: 'inlineshidden',
	install: true,
	version: meson.project_version()
)
