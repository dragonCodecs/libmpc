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

mpcencDeps = []
if isWindows
	libWinMM = c.find_library('winmm')
	mpcencDeps += libWinMM
endif

mpcenc = executable(
	'mpcenc',
	mpcencSrcs,
	include_directories: [includes, libmpcencInc, libmpcpsyInc] + extraIncs,
	link_with: [common, libmpcenc, libmpcpsy] + extraLibs,
	dependencies: [maths] + mpcencDeps,
	gnu_symbol_visibility: 'inlineshidden',
	install: true
)
