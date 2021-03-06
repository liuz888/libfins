# Libfins API Reference

### `finslib_connection_data_read( sys, unitdata, start_unit, num_units );`

### Parameters

| Parameter | Type | Description |
| :--- | :--- | :--- |
|**`sys`**|`struct fins_sys_tp *`|A pointer to a structure with the FINS context|
|**`unitdata`**|`struct fins_unitdata_tp *`|A pointer to the location where the unit data read from a remote PLC must be stored|
|**`start_unit`**|`uint8_t`|The first unit from which the unit information should be read|
|**`num_units`**|`size_t *`|The maximum number unit information blocks to return. At function return this contains the actual number of unit information blocks read|

### Return Value

| Type | Description |
| :--- | :--- |
|`int`|A return value from the list [`FINS_RETVAL_...`](fins_retval.md) indicating the result of the query|

### Description

### See Also

* [`FINS_RETVAL...`](fins_retval.md) &ndash; Libfins function return code list
* [`finslib_cpu_unit_data_read();`](finslib_cpu_unit_data_read.md)
* [`finslib_cpu_unit_status_read();`](finslib_cpu_unit_status_read.md)
