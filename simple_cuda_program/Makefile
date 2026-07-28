# SPDX-License-Identifier: GPL-3.0-or-later
#
# Makefile — Simple CUDA vector addition example
# Copyright (C) 2026 Markus Oppel, University of Vienna
#
# This program is free software: you can redistribute it and/or modify
# it under the terms of the GNU General Public License as published by
# the Free Software Foundation, either version 3 of the License, or
# (at your option) any later version.
#
# This program is distributed in the hope that it will be useful,
# but WITHOUT ANY WARRANTY; without even the implied warranty of
# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
# GNU General Public License for more details.
#
# You should have received a copy of the GNU General Public License
# along with this program.  If not, see <https://www.gnu.org/licenses/>.

CXX := nvcc
TARGET := vector_add
SRC := vector_add.cu

.PHONY: all clean

all: $(TARGET)

$(TARGET): $(SRC)
	$(CXX) -o $@ $^

run: $(TARGET)
	./$(TARGET)

clean:
	rm -f $(TARGET)