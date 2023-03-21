# SPDX-License-Identifier: BSD-3-Clause
# SPDX-FileCopyrightText: 2023 Rachel Mant <git@dragonmux.network>
mpccut = executable(
	'mpccut',
	['mpccut.c'],
	include_directories: includes,
	link_with: [common, libmpcdec, libmpcenc],
	dependencies: [maths],
	gnu_symbol_visibility: 'inlineshidden',
	install: true
)
