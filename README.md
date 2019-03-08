# Rust MAX3010x High-Sensitivity Pulse Oximeter and Heart-Rate Sensor for Wearable Health Driver

[![crates.io](https://img.shields.io/crates/v/max3010x.svg)](https://crates.io/crates/max3010x)
[![Docs](https://docs.rs/max3010x/badge.svg)](https://docs.rs/max3010x)
[![Build Status](https://travis-ci.org/eldruin/max3010x-rs.svg?branch=master)](https://travis-ci.org/eldruin/max3010x-rs)
[![Coverage Status](https://coveralls.io/repos/github/eldruin/max3010x-rs/badge.svg?branch=master)](https://coveralls.io/github/eldruin/max3010x-rs?branch=master)
![Maintenance Intention](https://img.shields.io/badge/maintenance-actively--developed-brightgreen.svg)

This is a platform agnostic Rust driver for the MAX3010x high-sensitivity
pulse oximeter and heart-rate sensor for wearable health, based on the
[`embedded-hal`](https://github.com/rust-embedded/embedded-hal) traits.

This driver allows you to:
- Get the number of samples available on the FIFO. See `get_available_sample_count()`.
- Get the number of samples lost from the FIFO. See `get_overflow_sample_count()`.
- Read samples from the FIFO. See `read_fifo()`.
- Perform a temperature measurement. See `read_temperature()`.
- Change into heart-rate, oximeter or multi-LED modes. See `into_multi_led()`.
- Set the sample averaging. See `set_sample_averaging()`.
- Set the LED pulse amplitude. See `set_pulse_amplitude()`.
- Set the LED pulse width. See `set_pulse_width()`.
- Set the sampling rate. See `set_sampling_rate()`.
- Set the ADC range. See `set_adc_range()`.
- Set the LED time slots in multi-LED mode. `set_led_time_slots()`.
- Enable/disable the FIFO rollover. See `enable_fifo_rollover()`.
- Clear the FIFO. See `clear_fifo()`.
- Wake-up and shutdown the device. See `shutdown()`.
- Perform a software reset. See `reset()`.
- Get the device part and revision id. See `get_part_id()`.
- Interrupts:
  - Read the status of all interrupts. See `read_interrupt_status()`.
  - Set FIFO-almost-full level interrupt. See `set_fifo_almost_full_level_interrupt()`.
  - Enable/disable the FIFO-almost-full interrupt. See `enable_fifo_almost_full_interrupt()`.
  - Enable/disable the ambient-light-cancellation overflow interrupt. See `enable_alc_overflow_interrupt()`.
  - Enable/disable the temperature-ready interrupt. See `enable_temperature_ready_interrupt()`.
  - Enable/disable the new-FIFO-data-ready interrupt. See `enable_new_fifo_data_ready_interrupt()`.


## The device
TODO
Datasheet:
- TODO

This driver should be compatible at least with the devices: MAX30102.

### Usage

Please find additional examples using hardware in this repository: [driver-examples]

[driver-examples]: https://github.com/eldruin/driver-examples

```rust
// TODO
```

## Support

For questions, issues, feature requests, and other changes, please file an
[issue in the github project](https://github.com/eldruin/max3010x-rs/issues).

## License

Licensed under either of

 * Apache License, Version 2.0 ([LICENSE-APACHE](LICENSE-APACHE) or
   http://www.apache.org/licenses/LICENSE-2.0)
 * MIT license ([LICENSE-MIT](LICENSE-MIT) or
   http://opensource.org/licenses/MIT) at your option.

### Contributing

Unless you explicitly state otherwise, any contribution intentionally submitted
for inclusion in the work by you, as defined in the Apache-2.0 license, shall
be dual licensed as above, without any additional terms or conditions.

