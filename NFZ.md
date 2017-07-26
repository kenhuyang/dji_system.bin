Never mind the fact that we are *seemingly* being forced into certain firmware variants as a *reaction* to CopterSafe NFZ bypass.

![You do not have to update the firmware and app if you don't want to](https://pbs.twimg.com/media/DE5s4L6VwAAzcKL.jpg)

![You do not have to update the firmware and app if you don't want to](https://pbs.twimg.com/media/DEVX8wyXgAAM8ox.jpg)

https://www.dji.com/newsroom/news/dji-updates-process-for-activating-software-and-firmware-updates
```
DJI Updates Process For Activating Software And Firmware Updates New Procedure Requires Login After Update; Password Reset Available
```

```
If this activation process is not performed, the aircraft will not have access to the correct geospatial information and flight functions for that region, 
and its operations will be restricted if you update the upcoming firmware: Live camera streaming will be disabled, and flight will be limited to a 50-meter 
(164-foot) radius up to 30 meters (98 feet) high.

The feature applies to all aircraft (mentioned above) that have been upgraded to the latest firmware or when using future versions of the DJI GO and GO 4 apps.
```

For posterity a bit of info on data_copy.bin aka the NFZ db abused by RedHerring

MD5 (data_copy.bin) = 133d14108497decbb85d79196ce703ca # example of an NFZ update 
```
$ ~/dji_research/tools/image.py nfz.sig 
{   'auth_key': b'GFAK',
    'blocks_cnt': 1,
    'enc_key': b'IAEK',
    'header_size': 224,
    'image_name': b'geof'
                  b'ense',
    'magic': b'IM*H',
    'payload_size': 2928640,
    'rsa_sig_size': 256,
    'scramble_key': <__main__.c_ubyte_Array_16 object at 0x10612f598>,
    'sha256_payload': <__main__.c_ubyte_Array_32 object at 0x10612f620>,
    'version': 1}
Can't find enc_key IAEK
Unpacking block {   'attrib': 1,
    'name': b'GFDB',
    'output_size': 2928640,
    'start_offset': 0}

$ file nfz.db 
nfz.db: SQLite 3.x database

$ sqlite3 nfz.db .schema
CREATE TABLE airmap_geofence_polygons (
        area_id int,
        points  blob,
        country int,
        lat     int,
        lng     int,
        radius  int,
        shape  int,
        sub_area_id int,
        height      int,
        area_level  int
      );
CREATE INDEX index_airmap_area_id on airmap_geofence_polygons (area_id);
CREATE INDEX index_airmap_lat_lng on airmap_geofence_polygons (lat, lng);
CREATE TABLE geofence_version (
        version            varchar(255),
        data_timestamp        int,
        area_count         int,
        remark varchar(255) DEFAULT NULL

      );

```


