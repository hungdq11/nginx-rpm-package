## nginx-rpm-package
Just nginx rpm package

## OpenSSL
* Rebuild NGINX with custom OpenSSL for HTTP/2 via ALPN
* built with OpenSSL 1.0.2l
## Dynamic module
Starting from NGINX 1.9.11, we can also compile module as a dynamic module and load the module in our ```nginx.conf``` via the [load_module](http://nginx.org/en/docs/ngx_core_module.html#load_module) directive, for example:
```
load_module /etc/nginx/modules/ngx_http_image_filter_module.so;
```
This build includes the following modules as dynamic modules:
* [lua-nginx-module](https://github.com/openresty/lua-nginx-module)
* [headers-more-nginx-module](https://github.com/openresty/headers-more-nginx-module)
* [echo-nginx-module](https://github.com/openresty/echo-nginx-module)
* [set-misc-nginx-module](https://github.com/openresty/set-misc-nginx-module)
* [nginx-rtmp-module](https://github.com/arut/nginx-rtmp-module)
* [nginx-push-stream-module](https://github.com/wandenberg/nginx-push-stream-module)
* [ngx_http_geoip_module](http://nginx.org/en/docs/http/ngx_http_geoip_module.html)
* [ngx_http_image_filter_module](http://nginx.org/en/docs/http/ngx_http_image_filter_module.html)
* [ngx_http_xslt_filter_module](http://nginx.org/en/docs/http/ngx_http_xslt_module.html)
