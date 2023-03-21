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
	c_args: '-DDLL_EXPORT',
	include_directories: includes,
	link_with: [common],
	dependencies: [maths],
	gnu_symbol_visibility: 'inlineshidden',
	name_prefix: '',
	install: true,
	version: meson.project_version()
)

libraryType = get_option('default_library')
libmpcdecArgs = []
if libraryType != 'static'
	libmpcdecArgs += '-DMPC_DLL_IMPORT'
endif

libmpcdec_dep = declare_dependency(
	compile_args: libmpcdecArgs,
	link_with: libmpcdec,
	include_directories: includes,
	version: meson.project_version()
)
