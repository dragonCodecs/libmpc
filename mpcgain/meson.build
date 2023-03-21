# SPDX-License-Identifier: BSD-3-Clause
# SPDX-FileCopyrightText: 2023 Rachel Mant <git@dragonmux.network>
mpcgain = executable(
	'mpcgain',
	['mpcgain.c'],
	include_directories: [includes] + extraIncs,
	link_with: [common] + extraLibs,
	dependencies: [maths, libreplaygain, libmpcdec_dep],
	gnu_symbol_visibility: 'inlineshidden',
	install: true
)
