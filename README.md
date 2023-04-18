## The Powershell script in this repository is responsible for parsing out Windows Event Log information for failed RDP attacks and using a third party API to collect geographic information about the attackers location.

## The script is used in this demo where I setup Azure Sentinel (SIEM) and connect it to a live virtual machine acting as a honey pot. We will observe live attacks (RDP Brute Force) from all around the world. I will use a custom PowerShell script to look up the attackers Geolocation information and plot it on an Azure Sentinel Map!

<image>

# Languages Used

    PowerShell: Extract RDP failed logon logs from Windows Event Viewer

# Utilities Used

    ipgeolocation.io: IP Address to Geolocation API

Attacks from China coming in; Custom logs being output with geodata

<image>

# World map of incoming attacks after 24 hours (built custom logs including geodata)
<image>
