# Vessel Scrubber Critical Parameter Sensor Analysis

## Introduction

Scrubbers, also known as Exhaust Gas Cleaning Systems (EGCS), play a crucial role in marine environments by removing particulate matter and harmful components, such as sulphur oxides (SOx) and nitrogen oxides (NOx), from exhaust gases produced during combustion processes in marine engines. This implementation of pollution control is essential for safeguarding human life and the environment against the adverse effects of toxic chemicals.

## Purpose

The primary purpose of scrubbing systems is to treat exhaust emissions from engines, auxiliary engines, and boilers both onshore and onboard marine vessels. This ensures that emissions meet specified environmental standards, preventing damage to both human health and the ecosystem.

## Compliance Parameters

For a vessel to be classified as compliant, it must satisfy four critical parameters:

1. **pH Value**
2. **PAH Value (Poly Aromatic Hydrocarbons)**
3. **Turbidity Difference**
4. **Gas Ratio**

## Compliance Sensors

Vessels are equipped with four sensors to measure and record these parameters. In the event of a sensor failure, a fifth sensor (virtual sensor) is employed to perform compliance checks as a fail-safe measure.


## Compliance Check

The compliance check involves ensuring that a vessel satisfies the defined parameters. Additionally, vessels operating in Emission Control Areas (ECA) are subject to more stringent compliance limits than those in global regions. Therefore, gas ratio checking is location-dependent, determined by the vessel's latitude and longitude.

## Implementation

The process begins with an ECA check to determine if the vessel is positioned within an ECA polygon. Following this, a compliance check is performed using a set of rules. To enhance accuracy, machine learning models are employed to predict missing values for the virtual sensor, ensuring comprehensive and reliable compliance assessments.

This integrated approach combines geographical considerations, compliance checks, and predictive modeling to create a robust and efficient scrubber system.

---

