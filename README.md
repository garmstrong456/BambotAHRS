# BambotAHRS

An AHRS library for the Idea7 Bambot. Based on Paul Stoffregen's MahonyAHRS library.

##Function Reference
#####begin(sampleFrequency)
Begin the AHRS filter using a fixed sample frequency. Only use this if you are sure your sketch will call the update function at fixed frequency. sampleFrequency is specified in Hz
#####update(gx, gy, gz, ax, ay, az, mx, my, mz, deltaT)
Update the orientation vector with new sensor data. Uses gyro, accellerometer and magnetometer data. deltaT is the elapsed time since the last call in seconds.
#####updateIMU(gx, gy, gz, ax, ay, az, deltaT)
Same as update, but only use gyro and accellerometer data.
#####getRoll(), getPitch(), getYaw()
Return the corresponding Euler angles in degrees
#####getRollRadians(), getPitchRadians(), getYawRadians()
Return the corresponding Euler angles in radians
