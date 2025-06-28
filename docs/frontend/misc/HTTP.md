### HTTP Protocol

_Hypertext Transfer Protocol_ (HTTP) adalah protokol yang berada di belakang World Wide Web (WWW). 
Protokol ini memungkinkan seseorang mengakses informasi dari web server yang berada di negara lain, dan menampilkan informasi tersebut ke perangkat komputer milik pribadi.

### URL Scheme 

_Uniform Resource Locator_ (URL) adalah rangkaian karakter yang digunakan sebagai penunjuk dari sebuah _resource_ yang ada di internet. URL sendiri terdiri dari beberapa bagian. Berikut ini adalah bagian-bagian URL.

```
<scheme>://<host>:<port>/<path>?=<query>#<fragment>
```

### HTTP Request Method

Tabel HTTP Request Method

| Method       | Deskripsi       | 
|---------------|---------------|
| GET   | Mengambil informasi / _resource_   |
| POST   | Mengupdate informasi / _resource_   |
| PUT   | Menyimpan informasi / _resource_   |
| DELETE   | Menghapus informasi / _resource_   |
| HEAD   | Mengambil informasi header atau metadata dari sebuah _resource_   |

### HTTP Header

#### HTTP Request Header 

Secara umum HTTP Request Header terdiri dari beberapa bagian berikut:

!!! info "Struktur HTTP Request Header"

    ```
    [HTTP Method] [URL] [HTTP Protocol Version]
    
    [Headers]
    
    [Body]
    ```
Berikut ini adalah isi dari HTTP Request Header
![HTTP Request Header](../asset/request_header.png)

#### HTTP Respone Header

HTTP Respone Header memiliki struktur yang mirip dengan HTTP Request Header. 
Berikut ini beberapa bagiannya:

!!! info "Struktur HTTP Respone Header"

    ```
    [HTTP Protocol Version] [Status Code] [Reason]

    [Header]

    [Body]
    ```
Berikut ini adalah isi dari HTTP Respone Header
![HTTP Respone Header](../asset/response_header.png)

### HTTP Response Status Code 

Tabel HTTP Respone Status Code

| Status Code       | Deskripsi       | 
|---------------|---------------|
| 1xx  | _Informational_   |
| 2xx   | _Succesful_   |
| 3xx   | _Redirection_   |
| 4xx   | _Client Error_   |
| 5xx   | _Server Error_   |

#### Common HTTP Status Code