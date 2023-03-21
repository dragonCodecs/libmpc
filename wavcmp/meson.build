# SPDX-License-Identifier: BSD-3-Clause
# SPDX-FileCopyrightText: 2023 Rachel Mant <git@dragonmux.network>
wavcmp = executable(
	'wavcmp',
	['wavcmp.c'],
	include_directories: [includes, libwavformatInc] + extraIncs,
	link_with: [common, libwavformat] + extraLibs,
	dependencies: [maths],
	gnu_symbol_visibility: 'inlineshidden',
	install: true
)
