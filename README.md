# 🧪 MoziChem Skills

This repository contains reusable skills for MoziChem workflows.

## 🧩 Available Skills

### 📘 `pythermodb-reference-maker`

Creates `pyThermoDB`-style YAML references from thermodynamic tables and correlations.

It is intended for turning source material into structured reference entries that can be used in thermodynamic datasets and model workflows. The skill helps organize both simple property tables and equation-based correlations into the YAML format expected by `pyThermoDB`.

Typical use cases include:

- converting tabulated reference data into YAML
- formatting correlation coefficients for properties such as heat capacity, vapor pressure, or density
- keeping table structure and metadata consistent with the target schema

The skill folder includes:

- `SKILL.md` for the main instructions
- `assets/` for YAML templates
- `references/` for supporting rules and examples
- `scripts/` for helper validation and conversion utilities

Supported inputs include:

- CSV
- PDF
- images
- raw text

## 📁 Structure

- `pythermodb-reference-maker/SKILL.md`
- `pythermodb-reference-maker/assets/`
- `pythermodb-reference-maker/references/`
- `pythermodb-reference-maker/scripts/`

## 📄 License

This project is licensed under the Apache License 2.0.

## ❓ FAQ

For any question, contact me on [LinkedIn](https://www.linkedin.com/in/sina-gilassi/)
