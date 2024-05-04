INCLUDE_DIRECTORIES("/usr/local/include")
LINK_DIRECTORIES("/usr/local/lib64")

MYSQL_ADD_PLUGIN(audit_connection
  audit_connection.cpp
  MODULE_ONLY
  MODULE_OUTPUT_NAME "audit_connection"
)

MYSQL_ADD_PLUGIN(maxdisk maxdisk.pp
  MODULE_ONLY MODULE_OUTPUT_NAME "maxdisk")