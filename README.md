# Swagger UI with css fixes

One `index.html` to render your swagger.yml file.


## How to use

1. Copy [index.html](https://raw.githubusercontent.com/reo7sp/swagger-ui-fancier/master/index.html) to folder with your swagger.yml file.

_On local machine:_

2. Run http server in folder with swagger.yml:
```sh
python3 -m http.server
# open http://localhost:8000 in your browser
```

_On production:_

2. Deploy nginx configuration:
```nginx
server {
    server_name docs.yourcompany.com;
    root /path/to/docs;
    expires -1;

    # auth_basic "docs";
    # auth_basic_user_file /path/to/htpasswd/file/docs.htpasswd;
}
```