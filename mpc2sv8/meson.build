# SPDX-License-Identifier: BSD-3-Clause
# SPDX-FileCopyrightText: 2023 Rachel Mant <git@dragonmux.network>
mpc2sv8 = executable(
	'mpc2sv8',
	['mpc2sv8.c'],
	include_directories: [includes] + extraIncs,
	link_with: [common, libmpcenc] + extraLibs,
	dependencies: [maths, libmpcdec_dep],
	gnu_symbol_visibility: 'inlineshidden',
	install: true
)
