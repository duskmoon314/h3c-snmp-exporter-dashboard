# h3c-snmp-exporter-dashboard

This repo contains files copied from my real-world usage of the `snmp-exporter` and Grafana to monitor an H3C router.

## Usage

1. Follow the guide of `snmp-exporter` to set up the exporter, but use the self-generated `snmp.yml` file from this repository.
2. Import dashboard JSON file into your Grafana instance.

### Notice

If you want to modify the `snmp.yml` file, follow the steps below:

1. Git clone `snmp_exporter` repository.
2. Backup the original `generator/generator.yml` file.
3. Copy the `generator.yml` file from this repository to the `generator/generator.yml` file.
4. Download MIB files from H3C's official website and place them in the `generator/mibs` directory.
5. Modify the `generator/generator.yml` file to include the MIB objects you want to monitor.
6. Generate the `snmp.yml` file following the instructions in the `snmp_exporter` repository.

