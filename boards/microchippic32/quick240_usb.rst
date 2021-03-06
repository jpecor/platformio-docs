..  Copyright (c) 2014-present PlatformIO <contact@platformio.org>
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
       http://www.apache.org/licenses/LICENSE-2.0
    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.

.. _board_microchippic32_quick240_usb:

Pontech Quick240
================

.. contents::

Hardware
--------

Platform :ref:`platform_microchippic32`: Microchip's 32-bit portfolio with the MIPS microAptiv or M4K core offer high performance microcontrollers, and all the tools needed to develop your embedded projects. PIC32 MCUs gives your application the processing power, memory and peripherals your design needs!

.. list-table::

  * - **Microcontroller**
    - 32MX795F512L
  * - **Frequency**
    - 80MHz
  * - **Flash**
    - 508KB
  * - **RAM**
    - 128KB
  * - **Vendor**
    - `Pontech <http://chipkit.net/wpcproduct/pontech-quick240/?utm_source=platformio&utm_medium=docs>`__


Configuration
-------------

Please use ``quick240_usb`` ID for :ref:`projectconf_env_board` option in :ref:`projectconf`:

.. code-block:: ini

  [env:quick240_usb]
  platform = microchippic32
  board = quick240_usb

You can override default Pontech Quick240 settings per build environment using
``board_***`` option, where ``***`` is a JSON object path from
board manifest `quick240_usb.json <https://github.com/platformio/platform-microchippic32/blob/master/boards/quick240_usb.json>`_. For example,
``board_build.mcu``, ``board_build.f_cpu``, etc.

.. code-block:: ini

  [env:quick240_usb]
  platform = microchippic32
  board = quick240_usb

  ; change microcontroller
  board_build.mcu = 32MX795F512L

  ; change MCU frequency
  board_build.f_cpu = 80000000L

Debugging
---------
:ref:`piodebug` currently does not support Pontech Quick240 board.

Frameworks
----------
.. list-table::
    :header-rows:  1

    * - Name
      - Description

    * - :ref:`framework_arduino`
      - Arduino Wiring-based Framework allows writing cross-platform software to control devices attached to a wide range of Arduino boards to create all kinds of creative coding, interactive objects, spaces or physical experiences.