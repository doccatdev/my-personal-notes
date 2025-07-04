### HTTP Protocol

_Hypertext Transfer Protocol_ (HTTP) adalah protokol yang berada di belakang World Wide Web (WWW). 
Protokol ini memungkinkan seseorang mengakses informasi dari web server yang berada di negara lain, dan menampilkan informasi tersebut ke perangkat komputer milik pribadi.

### URL Scheme 

_Uniform Resource Locator_ (URL) adalah rangkaian karakter yang digunakan sebagai penunjuk dari sebuah _resource_ yang ada di internet. URL sendiri terdiri dari beberapa bagian. Berikut ini adalah bagian-bagian URL.

```
<scheme>://<host>:<port>/<path>?<query string/parameter>#<fragment>
```

#### Example Part of URL

```
https://www.example.com:443/blog/article/search?docid=720&hl=en#dayone

```

!!! note "Catatan untuk paramter / query string"

Format dasar dalam paramter / query string adalah sebagai berikut:

`?key1=value2&key2=value2`

- Pasangan data ditulis dalam format `key=value`
- Jika memiliki lebih dari satu parameter dipisahkan dengan tanda `&`


### HTTP Request Method

Tabel HTTP Request Method

| Method       | Deskripsi       | 
|---------------|---------------|
| GET   | Mengambil data |
| POST   | Mengirimkan atau menambah data baru  |
| PUT   | Mengganti atau menimpa (_overwirte_) data |
| DELETE   | Menghapus data  |
| PATCH   | Mengganti atau mengubah sebagian data  |
| HEAD   | Mengambil informasi header atau metadata dari sebuah data   |


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
| 100-199  | _Informational_   |
| 200-299   | _Succesful_   |
| 300-399   | _Redirection_   |
| 400-499   | _Client Error_   |
| 500-599   | _Server Error_   |

#### Common HTTP Status Code
