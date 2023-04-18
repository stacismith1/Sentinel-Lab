## The Powershell script in this repository is responsible for parsing out Windows Event Log information for failed RDP attacks and using a third party API to collect geographic information about the attackers location.

### The script is used in this demo where I setup Azure Sentinel (SIEM) and connect it to a live VM honey pot. We will observe live attacks (RDP Brute Force) from all around the world. We will then use a custom PowerShell script to look up the attackers Geolocation information and plot it on an Azure Sentinel Map.

![IP_GPS_Lookup](https://user-images.githubusercontent.com/128299428/232877557-a17989be-f3f2-48d3-88f9-8e343dd9c519.png)

# Languages Used

    PowerShell: Extract RDP failed logon attempts from Windows Event Viewer logs

# Utilities Used

    ipgeolocation.io: IP Address to Geolocation API (API access is required)

# World map of incoming attacks after 24 hours (built custom logs including geodata)

![Geodata_world_map_attacks](https://user-images.githubusercontent.com/128299428/232878042-c71d0ed9-b6fa-4973-b1d0-1ccff8d67593.png)


