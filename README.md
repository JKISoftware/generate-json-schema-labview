# Generate JSON Schema LabVIEW

Simple example of generating [JSON Schema](https://json-schema.org) from LabVIEW data types.


## Goals

- To provide a starting point for generating a JSON Schema from a LabVIEW data type -- specifically, to be used in conjuction with the [JSONtext](https://www.vipm.io/package/jdp_science_jsontext/) and [JKI JSON Serialization](https://www.vipm.io/package/jki_lib_json_serialization/) libraries.
- To provide enough of a schema for interoperability with other software tools (typically non-LabVIEW tools) that can utilize JSON Schema for a variety of purposes like code generation, data validation, etc.

## Non-Goals
- This project does not aim to support all features of JSON Schema like validation, constraints, type references (`$ref`) and definitions (`$def`), etc.
- This project does not aim to create a validator (JSONtext already has one)
- This projecty does not aim to support all LabVIEW data types (but it would be nice to support all the types that JSONtext and JKI JSON Serialization support)

## Status

- Project Status: Example Code / Non-Production
- Save Version: LabVIEW 2020

![example](docs\images\example_front_panel.png)

## Roadmap

- [ ] Basic Data Types
  - [x] Array
  - [x] String
  - [x] Cluster
  - [x] Floating Points
  - [x] Integers
  - [ ] Path
  - [ ] Enums
  - [ ] Others
- [ ] Unit Tests

## Development

- Use LabVIEW 2020 or LabVIEW 2024+
- Install the required VI Packages using VIPM (see the `.vipc` and `.dragon` files for dependencies: JSONtext and OpenG Variant)
- Open `source\Generate JSON Schema.lvproj` and try running `source\Example Test JSON Schema.vi` (and experiment with changing the input data type)