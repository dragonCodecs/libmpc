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

subdir('include')
subdir('common')
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

libmpcdec_dep = declare_dependency(
	link_with: libmpcdec,
	include_directories: includes,
	version: meson.project_version()
)
