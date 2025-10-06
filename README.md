### Names: RUDAHIGWA MPARABANYI Loic

### ID: 28048
# Oracle Database Lab Report

## Overview of Tasks

### Created a Pluggable Database (PDB)

* PDB Name: LO_PDB_28048

* Admin User: LOIC_PLSQLAUCA_28048

* Purpose: To store all classwork and practice SQL tasks.

### Created and Deleted a PDB

* Temporary PDB Name: LO_to_delete_pdb_28048

* Demonstrated the creation and deletion of a PDB to understand database management tasks.

### Configured Oracle Enterprise Manager (OEM)

* Accessed OEM dashboard via browser.

* Verified PDB status and user accounts.

### Configured Oracle REST Data Services (ORDS)

* Enabled SQL Developer Web to interact with the PDB.

* Verified user schema and privileges.

## Notes / Issues Encountered

### ORDS SQL Developer Web showed “App unavailable”

* Cause: ORDS was not mapped to the PDB.

* Solution: Configured ORDS properly using the new ORDS 25.x CLI (ords install interactive --config C:\ords_conf) and ensured the PDB and user schema were open and granted proper privileges.

### Port 8080 was already in use

* Cause: Previous ORDS instance or other service using the port.

* Solution: Killed the process using taskkill /PID <PID> /F or switched ORDS to another port (8081).

### Configuration folder initially empty

* Cause: ORDS install was not executed correctly.

* Solution: Used correct syntax for ORDS 25.x interactive install with --config folder specified.
