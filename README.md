# nsx-i2c

`nsx-i2c` provides an optional NSX wrapper for Ambiq I2C and related register
driver helpers.

Purpose:
- preserve a migration-friendly `ns_i2c_*` API surface
- keep basic register-access helpers available for existing device code
- allow future sensor-specific drivers to depend on an NSX-managed I2C layer

This module is optional and intended for apps or higher-level modules that want
the legacy-style wrapper rather than direct HAL use.
