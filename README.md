# esp-matter-light-rgb
ESP-Matter application (with thread) for RGB light control on the ESP32c6

# Purpose
This project is a modified copy of the `espressif/esp-matter/examples/light` project. I wanted to understand features and clusters in code, and was able to figure out how to add an additional Hue and Saturation Feature to the Color Control Cluster.

# Helpfull References
## Matter Spec
- https://csa-iot.org/wp-content/uploads/2023/10/Matter-1.2-Standard-Namespace-Specification.pdf
- https://csa-iot.org/wp-content/uploads/2023/10/Matter-1.2-Device-Library-Specification.pdf
- https://csa-iot.org/wp-content/uploads/2023/10/Matter-1.2-Core-Specification.pdf
- https://csa-iot.org/wp-content/uploads/2023/10/Matter-1.2-Application-Cluster-Specification.pdf
- https://blog.espressif.com/matter-38ccf1d60bcd
- https://blog.espressif.com/matter-clusters-attributes-commands-82b8ec1640a0

# Thread
This project is default configured to use Thread on the `esp32c6`. If you wish to disable Thread, replace the `sdkconfig.defaults.esp32c6` file with `sdkconfig.defaults.c6_backup`

# Using this project
Follow the directions to install `esp-idf` and `esp-matter`. Pull this project's directory into that configured setup.