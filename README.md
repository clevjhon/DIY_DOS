# DIY DOS

Pre-release. ISBN 978-3-00-068463-0. ISSN: pending.

## Drive X: (backup / exchange) - concept, not yet implemented

X: is reserved for a network folder used for backups and file exchange.

Mapping (MS-DOS style):

    NET USE X: \\HOST\BACKUP

Backup of changed files from C:\DATA (archive attribute, then cleared):

    XCOPY C:\DATA X:\BACKUP\ /S /E /M /Y

Rules:

- X: is for backup and restore only; programs are not run from X:.
- If X: is not reachable, the backup stops with an error.
- No passwords are stored in AUTOEXEC.BAT or in this repository.
