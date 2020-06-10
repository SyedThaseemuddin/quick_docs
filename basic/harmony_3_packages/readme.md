---
title: Harmony 3 Packages
parent: Harmony Basics
has_toc: false
nav_order: 14
---

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[<img src="../../r_images/quick_home.png" title="Home">](../../readme.md) [<img src="../../r_images/quick_back.png"  title="Back">](../readme.md)
# Harmony 3 Packages

This page describes the packages that make up the MPLAB® Harmony software development framework. These packages are foundin the <a href="https://github.com/Microchip-MPLAB-Harmony" target="_blank">MPLAB  Harmony GitHub repository</a> and can be downloaded using the <a href="https://github.com/Microchip-MPLAB-Harmony/contentmanager/wiki" target="_blank">MPLAB Harmony 3 Content Manager</a>.


|  Package Name |  Descriptions | Example Function Names  |
| ---|---|---|
|  <a href="https://github.com/Microchip-MPLAB-Harmony/mhc" target="_blank">mhc</a> |Contains the implementation of the MPLAB Harmony Configurator (MHC) tool.	   | --   |
|  <a href="https://github.com/Microchip-MPLAB-Harmony/dev_packs" target="_blank">dev_packs</a> |Describes all peripherals, memory, etc. of each supported 32-bit device.	   | --    |
|  <a href="https://github.com/Microchip-MPLAB-Harmony/csp" target="_blank">csp</a> |Chip Support Package (CSP) supports initialization of Microchip 32-bit SAM and PIC® microcontroller and microprocessor devices. The peripheral libraries (PLIB) allow the development of simple applications that directly control the SAM and PIC peripherals.	   |UARTx_Initialize, UARTx_Read, TMRx_Start, TMRx_Stop, TCx_TimerStart, TCx_TimerStop, PORT_PinSet, PORT_PinRead   |
|  <a href="https://github.com/Microchip-MPLAB-Harmony/bsp" target="_blank">bsp</a> |Board Support Package (BSP) defines the name of the evaluation board and the name of switches and LEDs on the board. It also defines the attributes of the pins connected to the switches and LEDs (e.g.: data direction).	   | --   |
|  <a href="https://github.com/Microchip-MPLAB-Harmony/core" target="_blank">core</a> | Provides drivers and system services that have advanced capabilities and a higher level of abstraction that gives better hardware independence. The drivers and services provide abstracted interfaces that do not change from device to device. Peripheral Library (PLIB) interfaces, while providing lower overhead and more direct control, give no such guarantee. Applications written using driver and service APIs do not usually need to be modified if the device configuration is changed or even if a new Microchip MCU or MPU device is selected. This package also implements the Operating System Abstraction Layer (OSAL).	   | DRV_USART_Initialize, DRV_USART_ReadBuffer, DRV_I2C_Initialize, DRV_I2C_ReadTransfer, SYS_TIME_TimerCreate, SYS_TIME_TimerCounterGet, OSAL_Malloc   |
|  <a href="https://github.com/Microchip-MPLAB-Harmony/crypto" target="_blank">crypto</a> |The Cryptographic Library includes functions to perform encryption, decryption, hashing, authentication, and compression within the embedded application. Random number generation (RNG) functions are also provided. The library provides DES, 3DES, and AES for block cipher needs. Depending on the algorithm in use, CBC and CTR modes are supported.	   | CRYPT_RNG_Initialize, CRYPT_RNG_Get, CRYPT_ECC_KeySizeGet, CRYPT_SHA256_DataAdd |
|  <a href="https://github.com/Microchip-MPLAB-Harmony/gfx" target="_blank">gfx</a> |Contains the Aria Graphics library, the MPLAB Harmony Graphics Composer (MHGC) plug-in, the Display Manager plug-in. It also includes a simple quickstart application (Aria Quickstart) that provides a touch-enabled starting point for Aria Graphics development.	   | GFX_ActiveContext, GFX_Set, GFXU_StringFontIndexLookup |
|  <a href="https://github.com/Microchip-MPLAB-Harmony/gfx_apps" target="_blank">gfx_apps</a> |Contains all other (non-quickstart) Aria and Legato Graphics Library demonstration projects   | -- |
|  <a href="https://github.com/Microchip-MPLAB-Harmony/net" target="_blank">net</a> |Contains the MPLAB Harmony 3 Network Package (Net). The Net repo provides a free fast to market TCP/IP stack for Microchip 32-bit SAM and PIC microprocessor devices. The repo contains multiple applications that demonstrate communication over TCP/IP using well-known protocols like TCP, UDP, HTTP, SMTP, etc.   | TCPIP_STACK_Status, TCPIP_STACK_NetIsReady, TCPIP_TCP_ArrayPut |
|  <a href="https://github.com/Microchip-MPLAB-Harmony/usb" target="_blank">usb</a> | The USB module components provide USB middleware and drivers. It also includes a variety of USB-related firmware projects that demonstrate the capabilities of the MPLAB Harmony USB stack.   | USB_DEVICE_Attach, USB_DEVICE_EventHandlerSet, USB_HOST_CDC_AttachEventHandlerSet |
|  <a href="https://github.com/Microchip-MPLAB-Harmony/audio" target="_blank">audio</a> | Contains a variety of audio-related firmware projects that demonstrate the capabilities of the MPLAB Harmony audio offerings, drivers for hardware codecs that can be connected to development boards (e.g. WM8904 Codec Daughterboard), and a Board Support Package (BSP) Audio Template that can be used to make configuring a new audio project a matter of just a few mouse clicks.   | DRV_WM8904_Initialize, DRV_WM8904_BufferAddRead, DRV_WM8904_VolumeSet |
|  <a href="https://github.com/Microchip-MPLAB-Harmony/bt" target="_blank">bt</a> | Bluetooth-related firmware projects that demonstrate the capabilities of the MPLAB Harmony Bluetooth offerings, drivers for Bluetooth modules that can be connected to development boards (e.g. BM64 Bluetooth Module Daughterboard), and a BSP Bluetooth Template that can be used to make configuring a new Bluetooth project a matter of just a few mouse clicks.   | DRV_BM64_Open, DRV_BM64_BufferAddRead, DRV_BM64_VolumeSet |
|  <a href="https://github.com/Microchip-MPLAB-Harmony/motor_control" target="_blank">motor_control</a> | This module contains motor control demonstrations implemented on Microchip's 32-bit SAM microcontrollers. You can use these demonstrations as a reference for developing your own motor control applications. It also includes the X2C-Scope plug-in for the MPLAB® X IDE. X2C-Scope enables you to read, write, and plot global variables (for motor control) in real time. It communicates with the target using the UART.   | -- |
|  <a href="https://github.com/Microchip-MPLAB-Harmony/micrium_ucos3" target="_blank">micrium_ucos3</a> | This repository contains MPLAB Harmony configurations and applications for the Micrium OS-III. Micrium OS-III software is not included and must be downloaded separately.   | -- |
|  <a href="https://github.com/Microchip-MPLAB-Harmony/expresslogic_threadx" target="_blank">expresslogic_threadx</a> | This repository contains MPLAB Harmony configurations and demo applications for Threadx Real time operating system from Express Logic.   | -- |
|  <a href="https://github.com/Microchip-MPLAB-Harmony/touch" target="_blank">touch</a> | The Touch Library is a royalty-free library for developing touch applications on 32-bit microcontrollers with a Peripheral Touch Controller peripheral. You can use it to integrate the touch-sensing capability into your applications. The library supports both self-capacitance and mutual-capacitance acquisition methods.   | -- |
|  <a href="https://github.com/Microchip-MPLAB-Harmony/wireless" target="_blank">wireless</a> | This repository contains the MPLAB® Harmony 3 Wireless solutions and example applications. It helps quickly incorporate connectivity to designs with wireless ICs, modules, software and development kits that make connecting.    | -- |
|  <a href="https://github.com/Microchip-MPLAB-Harmony/aws_cloud" target="_blank">aws_cloud</a> | MPLAB® Harmony 3 Configurations and Applications to securely connect IoT devices to the AWS cloud using Amazon FreeRTOS.    | -- |
|  <a href="https://github.com/Microchip-MPLAB-Harmony/bootloader" target="_blank">bootloader</a> |This repository contains the MPLAB® Harmony 3 Bootloader. This can be used to upgrade the firmware on a target device without the need for an external programmer or debugger.    | bootloader_Trigger, bootloader_Start, run_Application  |
|  <a href="https://github.com/Microchip-MPLAB-Harmony/aerospace" target="_blank">aerospace</a> |This repository contains the MPLAB® Harmony 3 Aerospace solutions and example applications.  It helps  quickly incorporate connectivity to designs with Aerospace ICs, modules, software and development kits that make connecting effortless.    | --  |
|  <a href="https://github.com/Microchip-MPLAB-Harmony/cryptoauthlib_apps" target="_blank">cryptoauthlib_apps</a> |This repository contains the MPLAB® Harmony 3 CryptoAuthLib Applications solutions and example applications    | --  |
|  <a href="https://github.com/Microchip-MPLAB-Harmony/helix_mp3" target="_blank">helix_mp3</a> |This repository contains the MPLAB® Harmony 3 Helix MP3 Decoder Library. The source code is brought into a project automatically when the "Enable MP3 Decoder" checkbox is checked in the MHC Configuration Options for the Audio Decoder Libraries component of the Audio repository.    | --  |
|  <a href="https://github.com/Microchip-MPLAB-Harmony/CMSIS-FreeRTOS" target="_blank">CMSIS-FreeRTOS</a> |Cortex Microcontroller Software Interface Standard (CMSIS) FreeRTOS. By default, when Harmony 3 core or middleware libraries are used, the MPLAB Harmony Configurator (MHC) automatically includes FreeRTOS in order to provide more efficient use of the CPU. (RTOS use can still be disabled manually.)   | --  |
|  <a href="https://github.com/Microchip-MPLAB-Harmony/zlib" target="_blank">zlib</a> |A massively spiffy yet delicately unobtrusive compression library.   | --  |
|  <a href="https://github.com/Microchip-MPLAB-Harmony/wolfssl" target="_blank">wolfssl</a> |wolfSSL (formerly CyaSSL) is a small, fast, portable implementation of TLS/SSL for embedded devices to the cloud. wolfSSL supports up to TLS 1.3.   | --  |
|  <a href="https://github.com/Microchip-MPLAB-Harmony/wolfssh" target="_blank">wolfssh</a> |wolfSSH is a small, fast, portable SSH implementation, including support for SCP and SFTP.  | --  |
|  <a href="https://github.com/Microchip-MPLAB-Harmony/wolfMQTT" target="_blank">wolfMQTT</a> |This is an implementation of the MQTT Client written in C for embedded use, which supports SSL/TLS via the wolfSSL library. This library was built from the ground up to be multi-platform, space conscience and extensible. Integrates with wolfSSL to provide TLS support.  | --  |

## Reference Links
[<a href="https://www.microchip.com/design-centers/32-bit" target="_blank"> <img src="../../r_images/32_bit_mcus.png"> </a>]()  &nbsp; &nbsp; &nbsp; [<a href="https://www.microchip.com/design-centers/32-bit-mpus" target="_blank"> <img src="../../r_images/32_bit_mpus.png"> </a>]()  &nbsp; &nbsp; &nbsp; [<a href="https://www.microchip.com/mplab/mplab-x-ide" target="_blank"> <img src="../../r_images/mplab_x_ide.png"> </a>]()  &nbsp; &nbsp; [<a href="https://www.microchip.com/mplab/mplab-harmony" target="_blank"> <img src="../../r_images/mplab_harmony.png"> </a>]() [<a href="https://www.microchip.com/mplab/compilers" target="_blank"> <img src="../../r_images/mplab_compiler.png"> </a>]()  