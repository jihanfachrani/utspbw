## Dosen
<details>
<summary> Klik untuk Ekspan </summary>

### Create Dosen 
<table>
<tr>
    <td> <b>URL</b> </td>
    <td> {{baseURL}}/api/v1/dosen </td>
</tr>
<tr>
    <td> <b>Method</b> </td>
    <td> POST </td>
</tr>
<tr>
    <td> <b>Header</b> </td>
    <td> Authorization : Bearer Token  </td>
</tr>
<tr>
<td> <b>Body</b> </td>
<td>

``` json
{
    "nama" : "MASHUM ABDUL JABBAR",
    "alamat" : "Bogor"
}    
```

</td>
</tr>
<tr>
<td> <b>Respon Success</b> </td>
<td>

``` json
{
    "code" : 201,
    "message" : "Data Dosen berhasil diinput",
    "data" : {
        "id" : 1003,
        "nama" : "MASHUM ABDUL JABBAR",
        "alamat" : "Bogor"
    } 
}    
```

</td>
</tr>
<tr>
<td> <b>Respon Conflict</b> </td>
<td>

``` json
{
    "code" : 409,
    "message" : "Nama Dosen Telah digunakan",
    "data" : {
        "value" : "MASHUM ABDUL JABBAR",
        "property" : "nama",
        "location" : "body"
    } 
}    
```

</td>
</tr>
</table>


### Read Dosen By Id
<table>
<tr>
    <td> <b>URL</b> </td>
    <td> {{baseURL}}/api/v1/dosen </td>
</tr>
<tr>
    <td> <b>Example</b> </td>
    <td> {{baseURL}}/api/v1/dosen?id=1003 </td>
</tr>
<tr>
    <td> <b>Method</b> </td>
    <td> GET </td>
</tr>
<tr>
    <td> <b>Header</b> </td>
    <td> Authorization : Bearer Token  </td>
</tr>
<tr>
<td> <b>Query</b> </td>
<td> id=1003 </td>
</tr>
<tr>
<td> <b>Respon Success</b> </td>
<td>

``` json
{
    "code" : 200,
    "message" : "sukses",
    "data" : {
        "id" : 1003,
        "nama" : "MASHUM ABDUL JABBAR",
        "alamat" : "Bogor"
    } 
}    
```

</td>
</tr>
<tr>
<td> <b>Respon Not Found</b> </td>
<td>

``` json
{
    "code" : 404,
    "message" : "ID Dosen tidak ditemukan",
    "data" : {
        "value" : 1003,
        "property" : "id",
        "location" : "query"
    } 
}    
```

</td>
</tr>
</table>


### Read Dosen All
<table>
<tr>
    <td> <b>URL</b> </td>
    <td> {{baseURL}}/api/v1/dosen </td>
</tr>
<tr>
    <td> <b>Method</b> </td>
    <td> GET </td>
</tr>
<tr>
    <td> <b>Header</b> </td>
    <td> Authorization : Bearer Token  </td>
</tr>
<tr>
<td> <b>Respon Success</b> </td>
<td>

``` json
{
    "code" : 200,
    "message" : "Sukses",
    "data" : [
        {
            "id" : 1001,
            "nama" : "	MUHAMMAD ENCEP",
            "alamat" : "Bogor"
        },
        {
            "id" : 1002,
            "nama" : "HILMY ALIY ANDRA PUTRA",
            "alamat" : "Bogor"
        },
        {
            "id" : 1003,
            "nama" : "MASHUM ABDUL JABBAR",
            "alamat" : "Bogor"
        },
        {
            "id" : 1004,
            "nama" : "RISDIANTO IRAWAN",
            "alamat" : "Bogor"
        },
        {
            "id" : 1005,
            "nama" : "UUS FIRDAUS",
            "alamat" : "Bekasi"
        },
        {
            "id" : 1006,
            "nama" : "AZHARUDIN",
            "alamat" : "Bogor"
        },
        {
            "id" : 1007,
            "nama" : "MULIL KHAIRA",
            "alamat" : "Bogor"
        }
    ]
}    
```

</td>
</tr>
</table>

### Update Dosen
<table>
<tr>
    <td> <b>URL</b> </td>
    <td> {{baseURL}}/api/v1/dosen </td>
</tr>
<tr>
    <td> <b>Method</b> </td>
    <td> PUT </td>
</tr>
<tr>
    <td> <b>Header</b> </td>
    <td> Authorization : Bearer Token  </td>
</tr>
<tr>
<td> <b>Body</b> </td>
<td>

``` json
{
    "id" : 1005,
    "nama" : "UUS FIRDAUS",
    "alamat" : "Bogor"
}    
```

</td>
</tr>
<tr>
<td> <b>Respon Success</b> </td>
<td>

``` json
{
    "code" : 201,
    "message" : "Data Dosen Berhasil diubah",
    "data" : {
        "id" : 1005,
        "nama" : "UUS FIRDAUS",
        "alamat" : "Bekasi"
    } 
}    
```

</td>
</tr>
<tr>
<td> <b>Respon Conflict</b> </td>
<td>

``` json
{
    "code" : 409,
    "message" : "Nama Dosen Telah digunakan",
    "data" : {
        "value" : "UUS FIRDAUS",
        "property" : "nama",
        "location" : "body"
    } 
}    
```

</td>
</tr>
<tr>
<td> <b>Respon Not Found</b> </td>
<td>

``` json
{
    "code" : 404,
    "message" : "ID Dosen tidak ditemukan",
    "data" : {
        "value" : 1005,
        "property" : "id",
        "location" : "body"
    } 
}    
```

</td>
</tr>
</table>

### Delete Dosen
<table>
<tr>
    <td> <b>URL</b> </td>
    <td> {{baseURL}}/api/v1/dosen </td>
</tr>
<tr>
    <td> <b>Example</b> </td>
    <td> {{baseURL}}/api/v1/dosen?id=1003 </td>
</tr>
<tr>
    <td> <b>Method</b> </td>
    <td> DELETE </td>
</tr>
<tr>
    <td> <b>Header</b> </td>
    <td> Authorization : Bearer Token  </td>
</tr>
<tr>
<td> <b>Query</b> </td>
<td> id=1003 </td>
</tr>
<tr>
<td> <b>Respon Success</b> </td>
<td>

``` json
{
    "code" : 200,
    "message" : "Sukses dihapus",
    "data" : [] 
}    
```

</td>
</tr>
<tr>
<td> <b>Respon Not Found</b> </td>
<td>

``` json
{
    "code" : 404,
    "message" : "ID Dosen tidak ditemukan",
    "data" : {
        "value" : 1003,
        "property" : "id",
        "location" : "query"
    } 
}    
```

</td>
</tr>
</table>
</details>

## Mata Kuliah
<details>
<summary> Klik untuk Ekspan </summary>

### Create Mata kuliah
<table>
<tr>
    <td> <b>URL</b> </td>
    <td> {{baseURL}}/api/v1/matkul </td>
</tr>
<tr>
    <td> <b>Method</b> </td>
    <td> POST </td>
</tr>
<tr>
    <td> <b>Header</b> </td>
    <td> Authorization : Bearer Token  </td>
</tr>
<tr>
<td> <b>Body</b> </td>
<td>

``` json
{
    "matkul" : "Pemrograman Berbasis Web",
    "dosen penguji" : "MASHUM ABDUL JABBAR",
    "sks" : 3
}    
```

</td>
</tr>
<tr>
<td> <b>Respon Success</b> </td>
<td>

``` json
{
    "code" : 201,
    "message" : "Data Matkul Berhasil diinput",
    "data" : {
        "kodemk" : 01,
        "matkul" : "Pemrograman Berbasis Web",
        "dosen penguji" : "MASHUM ABDUL JABBAR",
        "sks" : 3
    } 
}    
```

</td>
</tr>
<tr>
<td> <b>Respon Conflict</b> </td>
<td>

``` json
{
    "code" : 409,
    "message" : "Nama Matkul Telah digunakan",
    "data" : {
        "value" : "Pemrograman Berbasis Web",
        "property" : "nama",
        "location" : "body"
    } 
}    
```

</td>
</tr>
</table>


### Read Matkul By Kodemk
<table>
<tr>
    <td> <b>URL</b> </td>
    <td> {{baseURL}}/api/v1/matkul </td>
</tr>
<tr>
    <td> <b>Example</b> </td>
    <td> {{baseURL}}/api/v1/matkul?kodemk=01 </td>
</tr>
<tr>
    <td> <b>Method</b> </td>
    <td> GET </td>
</tr>
<tr>
    <td> <b>Header</b> </td>
    <td> Authorization : Bearer Token  </td>
</tr>
<tr>
<td> <b>Query</b> </td>
<td> kodemk=01 </td>
</tr>
<tr>
<td> <b>Respon Success</b> </td>
<td>

``` json
{
    "code" : 200,
    "message" : "Sukses",
    "data" : {
        "kodemk" : 01,
        "nama" : "Pemrograman Berbasis Web",
        "dosen penguji" : "MASHUM ABDUL JABBAR",
        "sks" : 3
    } 
}    
```

</td>
</tr>
<tr>
<td> <b>Respon Not Found</b> </td>
<td>

``` json
{
    "code" : 404,
    "message" : "Kode Mata Kuliah tidak ditemukan",
    "data" : {
        "value" : 01,
        "property" : "kodemk",
        "location" : "query"
    } 
}    
```

</td>
</tr>
</table>


### Read Matkul All
<table>
<tr>
    <td> <b>URL</b> </td>
    <td> {{baseURL}}/api/v1/matkul </td>
</tr>
<tr>
    <td> <b>Method</b> </td>
    <td> GET </td>
</tr>
<tr>
    <td> <b>Header</b> </td>
    <td> Authorization : Bearer Token  </td>
</tr>
<tr>
<td> <b>Respon Success</b> </td>
<td>

``` json
{
    "code" : 200,
    "message" : "Sukses",
    "data" : [
        {
            "kodemk" : 01,
            "matkul" : "Pemrograman Berbasis Web",
            "dosen penguji" : "MASHUM ABDUL JABBAR",
            "sks" : 3
        },
        {
            "kodemk" : 02,
            "matkul" : "Basis Data 2",
            "dosen penguji" : "UUS FIRDAUS",
            "sks" : 3
        },
        {
            "kodemk" : 03,
            "matkul" : "JARINGAN KOMPUTER",
            "dosen penguji" : "AZHARUDIN",
            "sks" : 3
        },
        {
            "kodemk" : 04,
            "matkul" : "Aljabar Linear",
            "dosen penguji" : "HILMY ALIY ANDRA PUTRA",
            "sks" : 3
        }
    ]
}    
```

</td>
</tr>
</table>

### Update Matkul
<table>
<tr>
    <td> <b>URL</b> </td>
    <td> {{baseURL}}/api/v1/matkul </td>
</tr>
<tr>
    <td> <b>Method</b> </td>
    <td> PUT </td>
</tr>
<tr>
    <td> <b>Header</b> </td>
    <td> Authorization : Bearer Token  </td>
</tr>
<tr>
<td> <b>Body</b> </td>
<td>

``` json
{
    "kodemk" : 01,
    "matkul" : "BAHASA PEMROGRAMAN 2",
    "dosen penguji" : "MASHUM ABDUL JABBAR",
    "sks" : 4
}    
```

</td>
</tr>
<tr>
<td> <b>Respon Success</b> </td>
<td>

``` json
{
    "code" : 201,
    "message" : "Data Matkul Berhasil diubah",
    "data" : {
        "kodemk" : 01,
        "matkul" : "BAHASA PEMROGRAMAN 2",
        "dosen penguji" : "MASHUM ABDUL JABBAR",
        "sks" : 4
    } 
}    
```

</td>
</tr>
<tr>
<td> <b>Respon Conflict</b> </td>
<td>

``` json
{
    "code" : 409,
    "message" : "Nama Matkul Telah digunakan",
    "data" : {
        "value" : "BAHASA PEMROGRAMAN 2",
        "property" : "nama",
        "location" : "body"
    } 
}    
```

</td>
</tr>
<tr>
<td> <b>Respon Not Found</b> </td>
<td>

``` json
{
    "code" : 404,
    "message" : "Kode Mata Kuliah tidak ditemukan",
    "data" : {
        "value" : 01,
        "property" : "kodemk",
        "location" : "body"
    } 
}    
```

</td>
</tr>
</table>

### Delete Matkul
<table>
<tr>
    <td> <b>URL</b> </td>
    <td> {{baseURL}}/api/v1/matkul </td>
</tr>
<tr>
    <td> <b>Example</b> </td>
    <td> {{baseURL}}/api/v1/matkul?kodemk=01 </td>
</tr>
<tr>
    <td> <b>Method</b> </td>
    <td> DELETE </td>
</tr>
<tr>
    <td> <b>Header</b> </td>
    <td> Authorization : Bearer Token  </td>
</tr>
<tr>
<td> <b>Query</b> </td>
<td> kodemk=01 </td>
</tr>
<tr>
<td> <b>Respon Success</b> </td>
<td>

``` json
{
    "code" : 200,
    "message" : "Sukses dihapus",
    "data" : [] 
}    
```

</td>
</tr>
<tr>
<td> <b>Respon Not Found</b> </td>
<td>

``` json
{
    "code" : 404,
    "message" : "Kode Mata Kuliah tidak ditemukan",
    "data" : {
        "value" : 01,
        "property" : "kodemk",
        "location" : "query"
    } 
}    
```

</td>
</tr>
</table>
</details>