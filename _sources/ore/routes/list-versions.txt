=====================
List project versions
=====================

**GET /projects/:pluginId/versions**

Returns a list of versions for a project of a given plugin ID based on given criteria.

**Query parameters:**

+----------+-----------------------------+-------------------------------------------------------------+
| Name     | Data Type                   | Description                                                 |
+==========+=============================+=============================================================+
| channels | Comma Separated String List | Filters versions by channels (inclusive).                   |
+----------+-----------------------------+-------------------------------------------------------------+
| limit    | Integer                     | Limits the amount of versions returned (max / default: 10). |
+----------+-----------------------------+-------------------------------------------------------------+
| offset   | Integer                     | Drops the first *n* versions from the result list.          |
+----------+-----------------------------+-------------------------------------------------------------+
