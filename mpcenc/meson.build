# SPDX-License-Identifier: BSD-3-Clause
# SPDX-FileCopyrightText: 2023 Rachel Mant <git@dragonmux.network>
mpcencSrcs = [
	'mpcenc.c',
	'keyboard.c',
	'pipeopen.c',
	'stderr.c',
	'wave_in.c',
	'winmsg.c',
]

mpcenc = executable(
	'mpcenc',
	mpcencSrcs,
	include_directories: [includes, libmpcencInc, libmpcpsyInc],
	link_with: [common, libmpcenc, libmpcpsy],
	dependencies: [maths],
	gnu_symbol_visibility: 'inlineshidden',
	install: true
)
