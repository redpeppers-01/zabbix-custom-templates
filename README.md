# Zabbix Custom Templates Collection

This repository contains custom-built monitoring templates for Zabbix monitoring system, designed for telecommunications and data center environments.

## Available Templates

### DOCSIS Cable Modem Template
Location: [template_docsis_cable_modem/7.2/](template_docsis_cable_modem/7.2/)

A comprehensive SNMP monitoring template for DOCSIS cable modems providing extensive physical layer monitoring, security tracking, and performance metrics.

**Key Features:**
- Physical layer monitoring (signal power, SNR, microreflections)
- Advanced pre-equalization analysis with built-in JavaScript processing
- BPI+ security monitoring
- Performance metrics and error tracking
- DOCSIS 1.0-3.1 compatibility
- Self-contained design (no external scripts required)

[View Full Documentation →](template_docsis_cable_modem/7.2/README.md)

### ICEqube CMKT HVAC Template
Location: [template_ICEqube_CMKT/7.2/](template_ICEqube_CMKT/7.2/)

Comprehensive SNMP monitoring solution for ICEqube CMKT precision cooling units used in telecommunications huts, data centers, and edge computing sites.

**Key Features:**
- Complete HVAC health monitoring (10 fault items)
- Performance metrics (fan speeds, temperatures, voltage)
- Black-box availability monitoring (ICMP + SNMP)
- Flexible configuration with user macros
- Built-in dashboard for operational overview
- 100% manual trigger closure support

[View Full Documentation →](template_ICEqube_CMKT/7.2/README.md)

### BARD MC4000 Series HVAC Template
Location: [template_bard_4000_series_hvac/7.2/](template_bard_4000_series_hvac/7.2/)

Comprehensive SNMP monitoring template for BARD MC4000 Series precision HVAC controllers used in telecommunications shelters, data centers, and critical infrastructure environments.

**Key Features:**
- Dual-unit HVAC monitoring with lead/lag role tracking
- Multi-stage cooling (4 stages) and heating (4 stages) monitoring
- Critical safety monitoring (fire/smoke shutdown detection)
- Comprehensive fault detection (10 alarm items)
- Temperature monitoring (local + 2 remote sensors)
- Power loss detection for both units
- Built-in dashboard with system status overview

[View Full Documentation →](template_bard_4000_series_hvac/7.2/README.md)

## Repository Structure
```
.
├── template_docsis_cable_modem/
│   └── 7.2/
│       ├── README.md
│       ├── template_docsis_cable_modem.yaml
│       └── files/
│           └── img/
├── template_ICEqube_CMKT/
│   └── 7.2/
│       ├── README.md
│       ├── template_iceqube_cmkt.yaml
│       └── files/
│           └── img/
├── template_bard_4000_series_hvac/
│   └── 7.2/
│       ├── README.md
│       ├── template_bard_4000_series_hvac.yaml
│       └── files/
│           └── img/
└── README.md
```

## Requirements

- Zabbix Server 7.2 or newer
- SNMP access to monitored devices
- Network connectivity (ICMP and UDP 161)
- Valid SNMP community string or SNMPv3 credentials

## Installation

1. Download the desired template `.yaml` file
2. Import via Zabbix web interface (Configuration → Templates → Import)
3. Create/configure host with SNMP interface
4. Configure SNMP credentials in host macros
5. Link template to host
6. Verify data collection

For detailed setup instructions, refer to individual template README files.

## Contributing

1. Fork the repository
2. Create your feature branch
3. Commit your changes
4. Push to the branch
5. Create a new Pull Request

## License

This project is open source and available under the [MIT License](LICENSE).

## Contact

````bash
://echo@dla.network [oZark oRChes✝ra✝'d]
````

[☕ Buy me a coffee](https://www.buymeacoffee.com/p_pepp)

---

**Last Updated:** November 25, 2025