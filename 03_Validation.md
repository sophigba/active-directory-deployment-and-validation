# 3. Validation Methodology.

## 3.1 Why Brute Force?
To validate the end-to-end functionality of this lab, a Remote Desktop Protocol (RDP) Brute-Force Attack was selected as the testing mechanism. This method was chosen because it simultaneously tests multiple layers of the deployment:

* Connectivity: Confirms that the attacker can reach the Target-PC via the network.

* RDP Availability: Ensures the RDP service is correctly configured and listening for external requests.

* Telemetry Generation: Forces the generation of high-volume logs, providing the necessary data to test the Splunk ingestion pipeline.
