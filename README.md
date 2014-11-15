# backup-humax

Backup media directory from Humax PVR

This script backs up the media directories from a Humax PVR to a local disk.

It uses the FTP server on the Humax PVR, and copies all files provided by 
that server, to the local directory.

## Deleted programmes

The script mirrors the Humax, including file deletions. So, this backup
does not guard against accidentally deleting a programme unless you catch it
before the backup runs again.

## Encryption

PVR recordings are encrypted.  This script does not decrypt them,
it just copies the encrypted files.  These files can be restored to
the **same** PVR but are useless on another PVR.

## Archiving

Because of the two restrictions listed above, this script is not intended
for archiving.  It is primarily intended to protect against hard disk failures.

## Requirements

1. Humax PVR must have a network connection, with a known IP address.

2. Humax must be on (not just in standby) when the script runs.
You may want to run the script frequently so it can catch the Humax
when it is on.

3. FTP must be enabled on the Humax.

4. The script depends on `lftp` being installed.

## Notices
Copyright (c) 2014 Graham R. Cobb.
This software is distributed under the GPL (see the copyright notices and the LICENSE file).

`backup-humax` is free software; you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation; either version 2 of the License, or
(at your option) any later version.

`backup-humax` is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

**IMPORTANT NOTES:** Humax is a trademark of Humax Co. Ltd.
This page and software is not created, endorsed, reviewed, approved or in any other
way associated with Humax Co. Ltd.
