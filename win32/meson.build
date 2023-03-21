# SPDX-License-Identifier: BSD-3-Clause
# SPDX-FileCopyrightText: 2023 Rachel Mant <git@dragonmux.network>
win32Srcs = [
	'attgetopt.c',
	'basename.c',
	'dirent.c',
]
win32Inc = include_directories('.')

win32Lib = static_library(
	'win32',
	win32Srcs,
	include_directories: includes,
	gnu_symbol_visibility: 'inlineshidden',
	install: true
)

extraIncs += win32Inc
extraLibs += win32Lib
