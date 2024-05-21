---
title: icm20948_driver
date: 2024-05-19
authors:
  - name: Zachary Olkin
    link: https://github.com/Zolkin1
    image: https://github.com/Zolkin1.png
tags:
  - Code
  - Rust
  - Device Driver
---

## A device agnostic driver for the ICM-20948 IMU written in Rust
<!--more-->

This project is a ICM-20948 (Inertial Measurement Unit) device driver written in Rust. The driver uses the embedded-hal traits and thus can be used on any microcontroller that has a HAL that implements those traits. The source code can be found on [github](https://github.com/Zolkin1/icm20948_driver). Documentation can be found on the [docs.rs](https://docs.rs/icm20948_driver/0.1.0/icm20948_driver/) page. The data sheet for this device can be found [here](https://invensense.tdk.com/download-pdf/icm-20948-datasheet/). See the documentation for current limitations and future plans. Please create an issue on github or contact me if there are issues that need to be resolved.

I decided to start writing this driver to practice writing Rust and to provide an easy to use IMU driver for future projects. I hope to use it in my robotics projects.

I currently have plans to update the driver soon with changes as suggested in the Github Repo. Another blog post will be published when those changes go live.

## Relevant Links
[Github](https://github.com/Zolkin1/icm20948_driver)

[Docs.rs](https://docs.rs/icm20948_driver/0.1.0/icm20948_driver/)

[Crates.io](https://crates.io/crates/icm20948_driver)

[IMU Datasheet](https://invensense.tdk.com/download-pdf/icm-20948-datasheet/)