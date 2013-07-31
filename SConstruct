# SConstruct file for emulino
# Copyright 2009 Greg Hewgill
#
# This file is part of Emulino.
#
# Emulino is free software: you can redistribute it and/or modify
# it under the terms of the GNU General Public License as published by
# the Free Software Foundation, either version 3 of the License, or
# (at your option) any later version.
#
# Emulino is distributed in the hope that it will be useful,
# but WITHOUT ANY WARRANTY; without even the implied warranty of
# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
# GNU General Public License for more details.
#
# You should have received a copy of the GNU General Public License
# along with Emulino.  If not, see <http://www.gnu.org/licenses/>.

env = Environment(CFLAGS = "-Wall -Werror")
env.Program("emulino", ["emulino.c", "loader.c", "cpu.c", "eeprom.c", "port.c", "timer.c", "usart.c"])
env.Command("avr.inc", ["mkinst.py", "instructions.txt"], "/usr/bin/python2.7 mkinst.py")
