# Notes and References

## CSA Docs
- https://csa-iot.org/wp-content/uploads/2023/10/Matter-1.2-Standard-Namespace-Specification.pdf
- https://csa-iot.org/wp-content/uploads/2023/10/Matter-1.2-Device-Library-Specification.pdf
- https://csa-iot.org/wp-content/uploads/2023/10/Matter-1.2-Core-Specification.pdf
- https://csa-iot.org/wp-content/uploads/2023/10/Matter-1.2-Application-Cluster-Specification.pdf

## Espressif Blog/references
- https://blog.espressif.com/matter-38ccf1d60bcd
- https://blog.espressif.com/matter-clusters-attributes-commands-82b8ec1640a0

## Temp sensor notes

### From The CSA-provided Matter Specification, section `7.18.2.11`

This type, derived from int16, represents a temperature on the Celsius scale with a resolution of 0.01°C.

• value = (temperature in °C) x 100
```
• -4°C ⇒ -400
• 123.45°C ⇒ 12345
```

The range is constrained by absolute zero: -273.15°C to 327.67°C.

### Conversion of Temperature Values for Display

When converting temperature values for display manufacturers SHOULD ensure that calculations *round* to the nearest representable value. Particular care is needed when using integer arithmetic.