The command below will use tccprofile.py to generate a whitelist profile with the following characteristics:

Able to send restricted AppleEvents:

/Library/Application Support/JAMF/Jamf.app - Send AppleEvents to Microsoft AutoUpdate.app
/usr/local/jamf/bin/jamfAgent - Send AppleEvents to Microsoft AutoUpdate.app
/usr/local/jamf/bin/jamf - Send AppleEvents to Microsoft AutoUpdate.app

Command:

/path/to/tccprofile.py --apple-event "/Library/Application Support/JAMF/Jamf.app","/Library/Application Support/Microsoft/MAU2.0/Microsoft AutoUpdate.app" "/usr/local/jamf/bin/jamfAgent","/Library/Application Support/Microsoft/MAU2.0/Microsoft AutoUpdate.app" "/usr/local/jamf/bin/jamf","/Library/Application Support/Microsoft/MAU2.0/Microsoft AutoUpdate.app" --allow --payload-description="This profile allows Microsoft AutoUpdate management via Jamf." --payload-identifier="com.company.msautoupdate.jamf.management.tcc.privacy.whitelist" --payload-name="Privacy Settings Whitelist - Microsoft AutoUpdate Management" --payload-org="Company Name" -o Microsoft_AutoUpdate_Management_v1.mobileconfig
