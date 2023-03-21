# SPDX-License-Identifier: BSD-3-Clause
# SPDX-FileCopyrightText: 2023 Rachel Mant <git@dragonmux.network>
project(
	'libmpc',
	'c',
	version: '7.0.1',
	meson_version: '>= 0.63',
	subproject_dir: 'deps'
)

c = meson.get_compiler('c')
maths = c.find_library('m', required: false)
isWindows = target_machine.system() == 'windows'

libreplaygain = subproject(
	'libreplaygain',
).get_variable(
	'libreplaygain_dep'
)

libcuefile = subproject(
	'libcuefile',
).get_variable(
	'libcuefile_dep'
)

if cxx.get_id() == 'msvc'
	add_project_arguments('-D_CRT_SECURE_NO_WARNINGS', language: 'c')
endif

extraIncs = []
extraLibs = []

subdir('include')
subdir('common')
if isWindows
	subdir('win32')
endif
subdir('libmpcdec')
subdir('libmpcpsy')
subdir('libmpcenc')
subdir('libwavformat')
subdir('mpcgain')
subdir('mpcdec')
subdir('mpcenc')
subdir('mpc2sv8')
subdir('mpccut')
subdir('mpcchap')
subdir('wavcmp')
