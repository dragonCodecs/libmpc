# SPDX-License-Identifier: BSD-3-Clause
# SPDX-FileCopyrightText: 2023 Rachel Mant <git@dragonmux.network>
mpcdec = executable(
	'mpcdec',
	['mpcdec.c'],
	include_directories: [includes, libwavformatInc] + extraIncs,
	link_with: [common, libwavformat, libmpcdec] + extraLibs,
	dependencies: [maths],
	gnu_symbol_visibility: 'inlineshidden',
	install: true
)
