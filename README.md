# pchecker
different kinds of proxy server checking tool
# download
click [download](https://github.com/snail007/pchecker/releases)
## Usage
```text
Usage of ./pchecker:
  -cn
    	true: check baidu; false: check youtube (default true)
  -debug
    	in debug mode , errors will be writed into error.log
  -in string
    	proxy servers list file (default "proxy.dat")
  -prefix string
    	prefix of output line
  -subfix string
    	subfix of output line
  -v	show version
```

## list file's content
below rules are supported by proxy servers list file:  

```text
 http://username:password@host:port  
 http://host:port  
 https://username:password@host:port  
 https://host:port  
 socks5://username:password@host:port  
 socks5://host:port  
 socks5s://username:password@host:port  
 socks5s://host:port  
 ss://method:password@host:port
 ```
### attention
`https`  means:  http(s) proxies over TLS   
`socks5s` means:  socks5 proxies over TLS   
`username` and `password` must encode by `URL_ENCODE`  
