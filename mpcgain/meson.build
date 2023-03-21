# SPDX-License-Identifier: BSD-3-Clause
# SPDX-FileCopyrightText: 2023 Rachel Mant <git@dragonmux.network>
mpcgain = executable(
	'mpcgain',
	['mpcgain.c'],
	include_directories: includes,
	link_with: [common, libmpcdec],
	dependencies: [maths, libreplaygain],
	gnu_symbol_visibility: 'inlineshidden',
	install: true
)
