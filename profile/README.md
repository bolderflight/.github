# About
We're a team of former NASA and DoD researchers and flight test engineers. We develop flight control and data acquisition systems that we would like to use - flexible and easy to configure, tight integration with MATLAB and Simulink, and a strong focus on data quality, determinism, and robustness. Our products are focused on meeting the needs of the flight research, commercial UAS, and emergent eVTOL markets. If you're interested in our systems, please check out our [website](https://bolderflight.com/) or [contact us](mailto:info@bolderflight.com).

## Flight Software
Our Research Flight Management Units (FMU-R) for UAS use our own open-source software stack, which ensures good data quality, exceptional determinism, and a fixed latency between sensing and actuation. The software stack integrates with Vehicle Management System (VMS) software developed in Simulink or C++ and includes an open-source Simulink simulation for development, testing, and validation. MAV Link communication is support enabling telemetry and control from [QGroundControl](http://qgroundcontrol.com/) and [Mission Planner](https://ardupilot.org/planner/) ground stations.
  * [Build Tools](https://github.com/bolderflight/build-tools): how to configure an environment to build the flight software.
  * [Flight Software](https://github.com/bolderflight/spaaro): flight software and documentation.

## Arduino Compatible Libraries
Many of our sensor drivers and data processing libraries are compatible with Arduino and are available under a BSD-3 or MIT license.

### Sensors
  * [Invensense-IMU](https://github.com/bolderflight/invensense-imu): MPU-6500 and MPU-9250 IMUs.
  * [VectorNav](https://github.com/bolderflight/vector-nav): VN-100, VN-200, and VN-300 IMU/INS over SPI communication. 
  * [HG4930](https://github.com/bolderflight/hg4930): Honeywell HG4930 IMU driver over RS422.
  * [SBUS](https://github.com/bolderflight/sbus): Reading from SBUS receivers and sending commands to SBUS servos.
  * [uBlox](https://github.com/bolderflight/ublox): UBX packets from uBlox GNSS receivers.
  * [LIS3MDL](https://github.com/bolderflight/lis3mdl): Reading from the magnetometer.
  * [BMP3xy](https://github.com/bolderflight/bmp3): BMP3XY series static pressure transducers.
  * [BME280](https://github.com/bolderflight/bme280): BME280 environmental sensor.
  * [BMI088](https://github.com/bolderflight/bmi088-arduino): BMI088 6-axis IMU.
  * [MS4525DO](https://github.com/bolderflight/ms4525do): MS4525DO pressure transducers.
  * [AMS5915](https://github.com/bolderflight/ams5915): AMS5915 pressure transducers.
  * [AMS5812](https://github.com/bolderflight/ams5812): AMS5812 pressure transducers.
  * [Ainstein-USD1](https://github.com/bolderflight/ainstein-usd1): RADAR altimeter.
  * [MAX31865](https://github.com/bolderflight/max31865): RTD front-end driver.
  * [TruStability RSC](https://github.com/bolderflight/tru-stability-rsc): Honeywell TruStability RSC pressure transducer.
  * [Terabee TeraRanger Hub](https://github.com/bolderflight/terabee): Terabee TeraRanger hub time of flight sensor for ranging and obstacle avoidance.

### Data Processing
  * [Eigen](https://github.com/bolderflight/eigen/): Arduino port of the [Eigen matrix math library](https://eigen.tuxfamily.org/index.php?title=Main_Page).
  * [Circular Buffer](https://github.com/bolderflight/circle_buf): Circular buffer.
  * [Polytools](https://github.com/bolderflight/polytools): polyfit and polyval.
  * [Statistics](https://github.com/bolderflight/statistics): real-time and moving window statistics.
  * [MAT v4](https://github.com/bolderflight/mat_v4): write variables in MATLAB v4 mat file format from Eigen and C++ arrays, matrices, and vectors.
  * [Julian Date](https://github.com/bolderflight/juliandate): converts from year, month, day and hour, minute, second to a Julian date.
  * [Decimal Year](https://github.com/bolderflight/decyear): converts from year, month, day and hour, minute, second to a decimal year.

### Communication
  * [MAVLink](https://github.com/bolderflight/mavlink): an easier to use MAV Link implementation.
  * [Framing](https://github.com/bolderflight/framing): Frames packets with start byte, end byte, and checksum to make data transfer and storage easy.
  * [ULEB128](https://github.com/bolderflight/uleb128): Unsigned little endian base 128 (ULEB128) implementation, which stores arbitrarily large unsigned integers in a variable length format
  * [LEB128](https://github.com/bolderflight/leb128): Signed little endian base 128 (LEB128) implementation, which stores arbitrarily large signed integers in a variable length format.
  * [IMAP](https://github.com/bolderflight/imap): Computes the number of bytes, scale factor, and bias to map a floating point value to an integer, given a range and the desired precision, useful for compression.
  * [Checksum](https://github.com/bolderflight/checksum/): Implements a Fletcher16 checksum.


### Estimation and Control
  * [Filter](https://github.com/bolderflight/filter): Rational transfer function and IIR filters.
  * [Navigation](https://github.com/bolderflight/navigation): State estimation filters and navigation transforms.
  * [Air Data](https://github.com/bolderflight/airdata): Airspeed, altitude, temperature, and density.
  * [Control](https://github.com/bolderflight/control): Gain and PID control laws.
  * [Excitation](https://github.com/bolderflight/excitation): pulse, doublet, chirp, and multisine excitations.

