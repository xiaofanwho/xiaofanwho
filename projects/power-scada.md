# Conduit Power SCADA System on AWS

**Case studies:** [AWS](https://aws.amazon.com/solutions/case-studies/conduit-power-hitachi-energy-scada/) • [Hitachi Energy](https://www.hitachienergy.com/latam/es/news-and-events/customer-stories/how-conduit-power-manages-costs-by-operating-renewable-power-plants-remotely) • [Snapsoft](https://snapsoft.io/success-stories/Pioneering-Cloud-Based-SCADA-Conduit-Power's-Hitachi-SCADA-Launch-on-AWS)

Conduit Power partnered with Hitachi Energy to launch the first SCADA (Supervisory Control and Data Acquisition) system for power plants fully hosted on AWS in North America — letting operators monitor and control power plants remotely instead of running the SCADA system out of an on-site control room.

## My role

I managed the AWS side of the deployment: building and running the cloud infrastructure that hosts Hitachi Energy's SCADA software, and integrating it with Conduit Power's data platform (Supported by SnapSoft).

- Managed the deployment of the SCADA environment on AWS, coordinating with Hitachi Energy and other vendors to keep the rollout on schedule
- Migrated the power control (telemetry) database from AWS to Snowflake (dbt), including data modeling, Active Directory integration, and role-based access control
- Connected edge devices in the field (MQTT, Modbus, DNP3) into Snowflake, and built dbt models to process 10+ telemetry topics
- Built a daily reporting system that opened up telemetry data lake access across departments
- Responsible for the network-side configuration, connecting the offices, AWS, and remote power plant networks into a single secure architecture so telemetry and control traffic could flow reliably between the field and the cloud

## Why it mattered

Running SCADA on the cloud, rather than on local servers at each plant, let Conduit Power monitor and operate renewable power plants remotely — cutting the cost and overhead of staffing on-site control rooms while keeping the reliability and security a real-time power control system requires.
